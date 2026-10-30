# Arquitetura e integrações

## Estado de conhecimento

O site foi usado como aplicação online e foi descrito como mantendo dados online. As conversas disponíveis não identificam com segurança o framework, a linguagem, o banco de dados, o provedor de hospedagem ou o mecanismo de autenticação.

Por isso, este documento não presume uma stack técnica.

## Componentes lógicos do domínio

- Interface web.
- Gestão de despesas.
- Gestão de participantes e compartilhamento.
- Cálculo de rateios, saldos, pendências e repasses.
- Carteira e recebimentos.
- Painel de alunos.
- Integração de link de contato com WhatsApp.

Esta é uma decomposição funcional, não uma descrição comprovada dos serviços internos existentes.

## WhatsApp

Foi relatada uma ação “Enviar mensagem” no Painel de Alunos. O mecanismo exato precisa ser inspecionado. Não há confirmação de API oficial, webhook ou envio automático; pode ser apenas um link que abre uma conversa.

## Android, sincronização e push

Objetivos futuros registrados:
- Aplicativo Android instalável/APK.
- Uso em dois celulares Samsung.
- Sincronização de dados entre os dispositivos.
- Notificações push configuráveis.

Em 20/10/2026, APK, sincronização e Firebase ainda não estavam prontos. Portanto, Firebase não deve ser documentado como backend já implantado.

## SaaS

A visão de longo prazo considera transformar o produto em SaaS. Isso exige decisões futuras sobre:
- organizações/contas e isolamento de dados;
- usuários, convites, papéis e permissões;
- autenticação e recuperação de conta;
- planos, cobrança e limites;
- auditoria e segurança;
- backups, observabilidade e suporte.

## Inventário técnico a preencher

| Item | Estado |
|---|---|
| Framework frontend | Não identificado |
| Backend/API | Não identificado |
| Banco de dados | Não identificado |
| Autenticação | Não identificada |
| Hospedagem/deploy | Site online; provedor não identificado |
| WhatsApp | Ação de contato relatada; implementação a inspecionar |
| Firebase | Planejado; não confirmado como implantado |
| App Android/APK | Não concluído segundo conversa |
| Push | Planejado; não confirmado |

## Segurança

Nunca versionar .env, chaves de API, tokens, senhas, dados bancários ou dados pessoais de alunos. Usar variáveis de ambiente e permissões mínimas. Antes de tornar o repositório público, revisar histórico e arquivos para remover segredos e dados privados.
