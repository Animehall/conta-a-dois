# Essência do Produto — Conta a Dois

## 1. O que é

Conta a Dois é um espaço digital compartilhado para organizar a vida financeira e parte da rotina de duas pessoas. O produto deve reduzir dúvidas, desencontros e cálculos manuais: quem pagou, quem deve, o que é individual, o que é dos dois, o que está parcelado e quanto precisa ser acertado.

O produto não deve ser entendido apenas como uma planilha de despesas. Sua essência é oferecer uma visão clara, confiável e compartilhada da vida financeira do casal/dupla, sem apagar a autonomia financeira de cada pessoa.

## 2. Princípios que não podem se perder

1. **Clareza antes de complexidade:** valores, responsáveis, vencimentos e saldos precisam ser fáceis de entender.
2. **Individual e compartilhado coexistem:** nem toda despesa pertence aos dois. O sistema deve preservar essa distinção.
3. **Transparência:** cada lançamento precisa deixar claro quem registrou, quem pagou, quem é responsável e como foi dividido.
4. **Acerto justo:** a divisão padrão conhecida é 50/50 para despesas compartilhadas, mas a regra deve ser explícita e preparada para exceções futuras.
5. **Menos trabalho manual:** totais, parcelas, pendências e repasses devem ser calculados pelo sistema.
6. **Acesso compartilhado de verdade:** a experiência futura deve funcionar para duas contas/pessoas, e não depender de uma única pessoa operar tudo.
7. **Continuidade e segurança:** dados financeiros não podem se perder; alterações devem ser rastreáveis e protegidas.
8. **Interface prática:** priorizar leitura rápida, organização visual, tabelas compactas quando fizer sentido e ações claras.

## 3. Problema que resolve

Em uma vida compartilhada, pagamentos podem sair de contas, cartões ou carteiras diferentes. Sem uma visão única, é fácil perder a noção de:
- quanto cada pessoa pagou;
- quais gastos são pessoais e quais são compartilhados;
- quanto cada pessoa deveria assumir;
- quais parcelas ainda virão;
- quais valores estão pendentes;
- se existe repasse a fazer para equilibrar as contas.

O Conta a Dois deve transformar esses registros em uma visão organizada e compreensível.

## 4. Públicos e papéis

- **Pessoa A:** participante da conta compartilhada.
- **Pessoa B:** segundo participante, com autonomia para consultar e registrar informações conforme permissões.
- **Administrador/gestor do espaço:** papel conceitual para convidar participantes e gerenciar configurações. A implementação atual desse papel ainda precisa ser verificada.

Não presumir que nomes, e-mails ou identificadores de usuários devam ser fixos no código. A solução deve permitir configurar participantes.

## 5. Escopo conhecido do produto

### Núcleo financeiro compartilhado
- despesas individuais e compartilhadas;
- identificação de quem realizou/pagou a despesa;
- meios de pagamento, incluindo cartão e Pix;
- compras parceladas;
- pendências e repasses;
- cálculo de acertos entre participantes.

### Módulo Carteira / recebimentos
Em conversa de 21/10/2026, foi relatado um módulo Carteira com dashboard de recebimentos.

### Painel de Alunos
Também foi relatado:
- cadastro/gestão de alunos;
- mensalidades;
- pagamentos e outros ganhos;
- ação verde para enviar mensagem pelo WhatsApp;
- tabela compacta, com aparência de planilha/Excel.

A relação definitiva entre Carteira, Painel de Alunos e o núcleo de finanças domésticas precisa ser esclarecida no inventário do site. Não presumir que esses módulos compartilhem todas as mesmas regras.

## 6. Personalidade e experiência

O produto deve transmitir:
- organização;
- confiança;
- praticidade;
- transparência;
- parceria;
- controle sem burocracia.

A interface deve ser moderna e profissional, mas não excessivamente carregada. Evitar dashboards que exibam muitos números sem explicar o que significam. Cada indicador deve responder a uma pergunta útil.

## 7. O que o produto não deve fazer

- Misturar despesas pessoais com compartilhadas sem identificação.
- Tratar todo lançamento como divisão 50/50 automaticamente sem considerar seu tipo.
- Confundir valor pago com valor devido.
- Alterar retroativamente valores ou parcelas sem deixar claro o impacto.
- Expor dados financeiros de uma pessoa a terceiros sem autorização.
- Usar dados fictícios como se fossem dados reais.
- Guardar chaves de API, senhas ou credenciais no repositório.

## 8. Visão de evolução

A visão futura mencionada inclui:
- duas pessoas usando o sistema em dispositivos diferentes;
- sincronização online confiável;
- aplicativo Android instalável;
- notificações push;
- backend e infraestrutura Firebase, caso essa arquitetura seja validada;
- possibilidade de evolução para SaaS.

Esses itens são objetivos de evolução, não funcionalidades confirmadas como concluídas.

## 9. Regra para futuras IAs e desenvolvedores

Antes de propor uma mudança:
1. Leia este documento e os documentos de regras de negócio.
2. Inspecione o código real antes de decidir arquitetura ou reescrever módulos.
3. Preserve comportamentos existentes que estejam funcionando.
4. Não invente funcionalidades implementadas.
5. Registre decisões e atualize a documentação junto com o código.
6. Quando houver dúvida de regra financeira, não escolha silenciosamente: documente a dúvida e peça validação.
