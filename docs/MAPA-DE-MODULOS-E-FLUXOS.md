# Mapa de Módulos e Fluxos

Este mapa registra a organização funcional conhecida. É um mapa conceitual, não uma afirmação sobre a navegação atual ou nomes exatos de telas.

## 1. Núcleo financeiro compartilhado

### Despesas
Fluxo conceitual:
1. Pessoa registra uma despesa.
2. Informa descrição e valor.
3. Define se é individual ou compartilhada.
4. Identifica quem pagou e o meio de pagamento (por exemplo, cartão ou Pix).
5. Se parcelada, informa os dados de parcelamento.
6. O sistema atualiza os totais e responsabilidades.
7. A despesa aparece nos resumos e pendências correspondentes.

Campos que precisam ser confirmados no produto:
- descrição;
- valor total;
- data da compra;
- categoria;
- responsável/pagador;
- participantes responsáveis;
- tipo individual/compartilhada;
- meio de pagamento;
- cartão/conta de origem;
- número de parcelas;
- vencimentos;
- observações;
- estado (ativa, paga, cancelada etc.).

### Parcelas
O sistema precisa distinguir:
- valor total da compra;
- quantidade de parcelas;
- valor de cada parcela;
- parcelas já pagas;
- parcelas futuras;
- pessoa que pagou ou pagará;
- efeito da parcela no saldo de cada participante.

A fórmula e a política de arredondamento usadas atualmente ainda precisam ser inspecionadas.

### Pendências e repasses
Objetivo: demonstrar de forma transparente o desequilíbrio entre o que cada participante pagou e sua responsabilidade.

O sistema deve evitar confundir:
- despesa registrada;
- despesa paga;
- obrigação individual;
- obrigação compartilhada;
- valor já repassado;
- saldo ainda pendente.

A regra exata de cálculo deve ser validada com exemplos reais anonimizados antes de qualquer alteração.

## 2. Carteira / recebimentos

Relato de 21/10/2026: existe um módulo chamado Carteira com dashboard de recebimentos.

Perguntas de inventário:
- A Carteira registra entradas pessoais, da casa ou de uma atividade profissional?
- Os recebimentos alimentam o saldo geral?
- Há contas a receber, previsão e histórico?
- Como são classificados pagamentos e outros ganhos?
- Existe conciliação com despesas?

Não presumir respostas até inspecionar a aplicação.

## 3. Painel de Alunos

Relato de 21/10/2026:
- painel para acompanhar alunos;
- mensalidades;
- pagamentos;
- outros ganhos;
- botão/ação verde para enviar mensagem pelo WhatsApp;
- tabela compacta semelhante a uma planilha.

Fluxos a mapear:
- criar/editar aluno;
- registrar mensalidade;
- registrar pagamento;
- acompanhar situação de pagamento;
- registrar outros ganhos;
- abrir conversa no WhatsApp;
- filtrar, ordenar e localizar registros.

Campos e regras de alunos, vencimentos, atrasos, descontos e recorrência ainda precisam ser confirmados.

## 4. Acesso de duas pessoas

Objetivo: cada participante usar o sistema em seu próprio dispositivo, com dados sincronizados e permissões adequadas.

A validar:
- convite e aceite;
- identidade de cada participante;
- propriedade dos dados;
- permissões de leitura e edição;
- remoção de participante;
- resolução de edições simultâneas;
- auditoria de alterações.

## 5. Aplicativo Android

Objetivo futuro relatado:
- app instalável/APK;
- sincronização entre dois celulares Samsung;
- notificações push.

Ainda não há confirmação de tecnologia, empacotamento ou implementação.

## 6. Mapa de navegação a completar

| Área | Páginas/estados a documentar |
|---|---|
| Início/dashboard | visão geral, indicadores, atalhos, filtros |
| Despesas | lista, cadastro, edição, detalhe, exclusão |
| Parcelas | calendário/lista, detalhe, status |
| Pendências | resumo por pessoa, detalhes e histórico |
| Repasses | valor, origem, destino, data e confirmação |
| Carteira | recebimentos, totais, filtros, detalhes |
| Alunos | tabela, cadastro, edição, detalhe |
| Mensalidades | lançamentos, vencimentos, status |
| Configurações | participantes, preferências, categorias |
| Conta | autenticação, perfil e segurança |

Os nomes acima são categorias de inventário e podem não corresponder literalmente aos menus atuais.
