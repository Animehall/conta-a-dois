# Funcionalidades e módulos

Este documento separa o que foi relatado como presente no site do que ainda precisa ser validado.

## 1. Despesas

**Relatado como implementado**
- Lançamento e acompanhamento de despesas.
- Separação entre despesas individuais e compartilhadas.
- Identificação da pessoa associada à despesa.
- Registro do meio de pagamento, incluindo cartão e Pix.
- Suporte a despesas parceladas.

**Detalhes ainda a confirmar no código**
- Campos obrigatórios de cada lançamento.
- Categorias disponíveis e possibilidade de criar categorias.
- Regras para edição e exclusão.
- Tratamento de estornos, pagamentos parciais e despesas recorrentes.
- Como são calculadas e exibidas as parcelas futuras.

## 2. Despesas compartilhadas, pendências e repasses

**Relatado como implementado**
- Acompanhamento de despesas compartilhadas.
- Visualização de pendências entre as pessoas.
- Registro/acompanhamento de repasses.
- Divisão de despesas com referência a um acerto 50/50.

**A validar**
- Se 50/50 é padrão fixo ou configurável por lançamento.
- Como o sistema calcula saldo devedor e credor.
- Se repasses podem ser parciais.
- Como o sistema evita contar um repasse como nova despesa.
- Como são tratados ajustes e pagamentos feitos fora do sistema.

## 3. Carteira

**Relatado como implementado em 21/10/2026**
- Dashboard de recebimentos.
- Registro/acompanhamento de mensalidades.
- Registro de pagamentos e outros ganhos.
- Visão de valores recebidos.

**A validar**
- Campos, filtros e períodos do dashboard.
- Estados de pagamento (previsto, pendente, recebido, atrasado).
- Se há recorrência automática de mensalidades.
- Exportação e relatórios.

## 4. Painel de Alunos

**Relatado como implementado**
- Área para acompanhar alunos e mensalidades.
- Informações de pagamentos.
- Link/ação verde “Enviar mensagem” para abrir contato pelo WhatsApp.
- Tabela compacta, com apresentação semelhante a uma planilha/Excel, após ajuste solicitado.

**A validar**
- Cadastro e edição de alunos.
- Dados armazenados por aluno.
- Formato e conteúdo da mensagem enviada.
- Se o WhatsApp é aberto com texto pré-preenchido.
- Busca, ordenação e filtros da tabela.

## 5. Acesso e sincronização

- O site mantinha dados online, conforme relato da conversa.
- O acesso da segunda pessoa ainda dependia de convite/liberação naquele momento.
- Não há confirmação de que o app Android, APK, sincronização entre celulares ou push tenham sido entregues.

## 6. Critérios de validação

Para marcar um item como concluído no repositório, verificar a funcionalidade na versão executável ou no código-fonte. Não converter uma intenção de produto em funcionalidade existente apenas por constar no roadmap.
