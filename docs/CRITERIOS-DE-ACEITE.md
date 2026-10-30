# Critérios de Aceite e Testes Funcionais

Os exemplos abaixo são cenários de teste propostos. Não afirmam que a aplicação atual já se comporta assim. Validar as regras com o responsável pelo produto antes de transformar expectativas em testes automatizados definitivos.

## Despesas individuais

- Uma despesa marcada como individual deve permanecer atribuída à pessoa indicada.
- A despesa individual não deve gerar automaticamente obrigação para o outro participante.
- Dashboard, listas e detalhes devem apresentar o mesmo valor e responsável.

## Despesas compartilhadas

- Uma despesa compartilhada deve identificar explicitamente os participantes responsáveis.
- Na regra padrão 50/50, cada participante assume metade do valor, observando arredondamento em centavos.
- O sistema deve distinguir o valor pago do valor que cabe a cada participante.
- O resumo deve permitir entender quem pagou e se há acerto pendente.

## Exemplo de validação matemática

Despesa compartilhada de R$ 100,00, paga integralmente pela Pessoa A, com divisão 50/50:
- responsabilidade da Pessoa A: R$ 50,00;
- responsabilidade da Pessoa B: R$ 50,00;
- pagamento realizado por A: R$ 100,00;
- desequilíbrio inicial: A adiantou R$ 50,00 em nome de B.

Este exemplo é uma referência matemática para validar a regra, não uma afirmação sobre a fórmula implementada atualmente.

## Parcelas

- Total das parcelas deve reconciliar com o valor total da compra.
- O sistema deve identificar parcela, quantidade total e vencimento.
- Pagamento de uma parcela não pode marcar as demais como pagas.
- Alterações em compras parceladas devem deixar claro o efeito nas parcelas futuras.
- Casos de arredondamento devem ser cobertos por testes.

## Pendências e repasses

- Um repasse deve reduzir a pendência correspondente sem apagar a despesa.
- Repasses parciais devem manter o saldo restante correto, caso sejam suportados.
- Os dois participantes devem visualizar valores consistentes.
- O histórico deve permitir entender a origem de cada ajuste.

## Carteira e Painel de Alunos

- Totais exibidos devem corresponder aos lançamentos filtrados.
- Pagamento recebido deve atualizar o status da cobrança correspondente, conforme regra validada.
- A ação de WhatsApp deve usar o contato correto e uma mensagem segura.
- Tabela deve permanecer utilizável em telas menores.

## Acesso e sincronização

- Participante não autorizado não pode acessar dados do espaço.
- Alterações feitas por uma pessoa devem aparecer para a outra dentro do comportamento de sincronização definido.
- Erros de rede não devem causar duplicação silenciosa de lançamentos.
- Conflitos de edição devem ser tratados de forma explícita.

## Qualidade geral

- Formulários devem validar campos obrigatórios e valores inválidos.
- Estados de carregamento, vazio e erro devem ser claros.
- Interface deve ser responsiva.
- Ações destrutivas devem pedir confirmação.
- Testes automatizados devem cobrir regras financeiras críticas.
