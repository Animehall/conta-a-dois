# Modelo de Dados Conceitual

**Atenção:** este documento é uma proposta para orientar a inspeção e não representa o esquema real do banco atual. Não implementar migrações com base nele sem comparar com o banco existente e validar as regras.

## Entidades conceituais

### Espaço compartilhado
Representa o ambiente financeiro compartilhado.
- id
- nome
- moeda
- configurações
- criado_em

### Participante
Representa uma pessoa com acesso ao espaço.
- id
- nome de exibição
- identificador de autenticação
- estado do convite
- papel/permissões

### Despesa
- id
- espaço_id
- descrição
- valor_total
- data
- categoria_id
- tipo: individual ou compartilhada
- pagador_id
- meio_pagamento
- observações
- estado
- criado_por
- criado_em
- atualizado_em

### Responsabilidade da despesa
Permite representar quem deve assumir cada parte.
- id
- despesa_id
- participante_id
- valor_responsabilidade
- percentual_responsabilidade

Essa entidade é importante para não forçar a regra 50/50 em despesas individuais ou exceções.

### Parcelamento
- id
- despesa_id
- quantidade_parcelas
- valor_total
- política de arredondamento

### Parcela
- id
- parcelamento_id
- número
- valor
- vencimento
- estado
- data_pagamento
- pagador_id

### Repasse
- id
- espaço_id
- origem_participante_id
- destino_participante_id
- valor
- data
- estado
- observação
- criado_por

### Carteira / lançamento financeiro
- id
- tipo (recebimento, ganho ou outro tipo a confirmar)
- descrição
- valor
- data
- categoria
- origem
- estado

### Aluno
- id
- nome
- contato
- estado
- observações

### Mensalidade / cobrança
- id
- aluno_id
- descrição
- valor
- competência
- vencimento
- estado

### Pagamento recebido
- id
- aluno_id
- cobrança_id (quando aplicável)
- valor
- data
- meio_recebimento
- observação

## Relações conceituais

- Um espaço possui participantes.
- Um espaço possui despesas.
- Uma despesa pode ter uma ou mais responsabilidades.
- Uma despesa pode possuir parcelamento.
- Um parcelamento possui parcelas.
- Um espaço possui repasses.
- Alunos podem possuir cobranças e pagamentos.
- A relação entre Carteira, alunos e finanças domésticas deve ser definida após inspeção.

## Regras de integridade recomendadas

1. Valores monetários devem usar decimal exato ou inteiro em centavos; evitar ponto flutuante binário.
2. A soma das responsabilidades deve corresponder ao valor que está sendo distribuído, conforme a regra definida.
3. Arredondamentos de centavos devem ter política determinística.
4. Uma parcela paga não deve ser contabilizada novamente.
5. Repasse não deve apagar nem reescrever a despesa original.
6. Exclusões financeiras devem ser controladas; avaliar cancelamento/estorno e trilha de auditoria.
7. Datas devem ter política de fuso horário consistente.
8. Toda operação deve respeitar o espaço e as permissões do participante.

## Questões que exigem validação

- O 50/50 é regra fixa ou padrão configurável?
- Há despesas compartilhadas com percentuais diferentes?
- O pagador é necessariamente um dos responsáveis?
- Como lidar com compra parcelada no cartão quando a fatura é paga por outra pessoa?
- A pendência é calculada por competência, vencimento ou fluxo de caixa?
- Como registrar repasse parcial?
- O que acontece quando uma despesa é editada depois de parcelas pagas?
- Carteira e Painel de Alunos são parte do mesmo domínio ou módulos independentes?
