# Regras de negócio conhecidas

## 1. Individual versus compartilhado

Toda despesa deve ser interpretável como individual ou compartilhada. Uma despesa individual pertence a uma pessoa; uma compartilhada participa do acerto entre as pessoas.

**Pendente de validação:** nomes exatos dos campos e se uma despesa pode ter mais de dois participantes.

## 2. Divisão 50/50

O projeto foi definido com referência a divisão igualitária (50/50) das despesas compartilhadas.

Exemplo conceitual, não especificação de cálculo validada: se uma despesa compartilhada elegível for de R$ 100, cada participante assume R$ 50. Se uma pessoa pagou os R$ 100, o acerto deve refletir a parte devida pela outra.

**Pendente de validação:** se há exceções, percentuais personalizados, arredondamento e tratamento de despesas pagas por mais de uma pessoa.

## 3. Pagamento e meio de pagamento

O histórico do projeto menciona cartão e Pix. O meio de pagamento deve ser distinguido da categoria da despesa e da pessoa responsável pelo pagamento.

**Pendente de validação:** suporte a dinheiro, débito, crédito, múltiplos cartões, contas bancárias e datas de vencimento.

## 4. Parcelamentos

O sistema foi descrito como possuindo suporte a parcelas. É necessário confirmar como o valor total, número de parcelas, valor por parcela e meses futuros são persistidos e exibidos.

**Pendente de validação:** antecipação, cancelamento, juros, parcelas variáveis e compras parceladas compartilhadas.

## 5. Pendências e repasses

Pendência representa saldo de acerto; repasse representa movimentação para liquidar esse saldo. Um repasse não deve ser tratado automaticamente como uma nova despesa de consumo.

**Pendente de validação:** algoritmo real, liquidação parcial, histórico de repasses, estornos e conciliação.

## 6. Carteira e mensalidades

A Carteira contempla recebimentos, mensalidades, pagamentos e outros ganhos. O Painel de Alunos permite acompanhar mensalidades e acionar contato por WhatsApp.

**Pendente de validação:** regras de vencimento, inadimplência, recorrência, descontos, pagamentos parciais e comprovantes.

## 7. Princípios de integridade

- Não misturar finanças pessoais com o saldo compartilhado.
- Não contar o mesmo evento duas vezes (despesa versus repasse).
- Preservar histórico de alterações financeiras quando a arquitetura permitir.
- Não expor dados de uma pessoa à outra sem a regra de compartilhamento correspondente.
- Não registrar senhas, tokens ou dados bancários sensíveis em arquivos versionados.

Estas são diretrizes para evolução; devem ser comparadas com o comportamento atual antes de qualquer refatoração.
