# Visão geral — Conta a Dois

## Propósito

O Conta a Dois nasceu como uma ferramenta para organizar a vida financeira de duas pessoas, separando o que é individual do que é compartilhado e facilitando a visualização de responsabilidades e acertos.

As pessoas citadas na definição inicial do projeto são Marcus e Mariana.

## Problemas que o produto busca resolver

1. Saber quanto cada pessoa gastou.
2. Distinguir despesas pessoais das despesas da casa e de outros compromissos compartilhados.
3. Registrar como cada despesa foi paga (por exemplo, cartão ou Pix).
4. Acompanhar compras parceladas.
5. Identificar quem pagou uma despesa compartilhada e quanto cabe a cada pessoa.
6. Visualizar pendências e repasses necessários para equilibrar as contas.
7. Reunir, em uma área separada, recebimentos, mensalidades e informações de alunos.

## Organização conceitual

- **Individual:** lançamento que pertence a apenas uma pessoa.
- **Compartilhado:** lançamento que deve ser considerado no acerto entre as duas pessoas.
- **Responsável pelo pagamento:** pessoa que efetivamente pagou ou registrou o pagamento.
- **Participantes do rateio:** pessoas às quais a despesa compartilhada é atribuída.
- **Pendência:** valor ainda devido no acerto entre participantes.
- **Repasse:** transferência feita para compensar valores pagos por outra pessoa.

Essas definições descrevem o domínio do produto. A implementação exata deve ser confirmada no código original.

## Módulos conhecidos

1. Controle de despesas.
2. Rateio, pendências e repasses.
3. Carteira/recebimentos.
4. Painel de Alunos.

## Público e acesso

O uso inicial foi pensado para duas pessoas. Em conversa de outubro de 2026, o acesso da segunda pessoa ainda dependia de convite ou liberação; portanto, não se deve assumir que havia autenticação multiusuário independente plenamente concluída.

## Produto futuro

A direção desejada inclui aplicativo Android instalável, uso em dois celulares, sincronização e notificações push. A intenção de longo prazo também inclui estruturar o produto como SaaS. Esses itens são objetivos futuros, não entregas confirmadas.
