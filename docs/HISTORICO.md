# Histórico do projeto

## 20/10/2026 — Definição do produto

- Projeto direcionado ao controle financeiro pessoal e compartilhado.
- Escopo citado: casa, carro, cartões/Pix, despesas, tarefas e acerto 50/50.
- Pessoas mencionadas no uso inicial: Marcus e Mariana.
- Visão futura: app Android instalável, notificações push e estrutura SaaS.
- APK, sincronização e Firebase ainda não estavam prontos naquele momento.

## 20/10/2026 — Site e módulos financeiros

- Site registrado: https://conta-a-dois-marcus.nexoraconceito.chatgpt.site
- Foi relatado controle de despesas por pessoa e meio de pagamento, incluindo cartão e Pix.
- Foram mencionados parcelamentos, despesas individuais/compartilhadas, pendências e repasses.
- Foi relatado que os dados ficavam online.
- Acesso da segunda pessoa ainda dependia de convite/liberação.

## 21/10/2026 — Carteira e Painel de Alunos

- Foi relatada implementação de dashboard de recebimentos.
- Painel de Alunos com mensalidades, pagamentos e outros ganhos.
- Ação verde “Enviar mensagem” para WhatsApp.
- Posteriormente foi aplicada tabela compacta, semelhante a uma planilha/Excel.

## 30/10/2026 — Criação do repositório

- Criado o repositório privado Animehall/conta-a-dois.
- Branch padrão: main.
- Repositório inicialmente vazio.
- Início da documentação de produto e regras com base no histórico disponível.

## 02/11/2026 — Recriação do app em arquivo único

- Código original não recuperado; criado `index.html` (HTML/CSS/JS puro, sem dependências externas) a partir dos docs do repo.
- **Confirmado (testado em navegador):** despesas individuais/compartilhadas, parcelas (centavos que sobram vão para as primeiras parcelas), rateio 50/50, repasses parciais, Carteira com totais, Painel de Alunos com tabela compacta e botão verde de WhatsApp, backup JSON.
- **Decisões tomadas (validar com o Marcus):** (1) só *parcelas pagas* de despesas compartilhadas entram no acerto; (2) o centavo ímpar do 50/50 fica com quem pagou; (3) repasse nunca vira despesa; (4) mensalidades recebidas somam na Carteira como linha separada.
- **Fora do escopo desta versão:** login/convite, sincronização entre aparelhos, Android/APK, push, Firebase.
- Nota: um prompt externo (Gemini) descrevia uma landing page romântica rosa/dourada; foi descartado em favor dos docs (app de finanças, branco + roxo/lilás).

## Observação

Este histórico é parcial e baseado nas conversas recuperadas. Adicionar novas decisões com data, contexto, decisão tomada e impacto. Diferenciar sempre implementação confirmada, relato histórico, hipótese e planejamento.
