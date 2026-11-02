# Conta a Dois

Projeto de organização financeira e gestão compartilhada do cotidiano de duas pessoas.

> **Estado deste repositório:** documentação do projeto + uma **recriação** do app em `index.html` (arquivo único, abre direto no navegador). O código-fonte original do site publicado não foi recuperado; a recriação segue os docs e **não é cópia** do original. Compare com a versão publicada antes de substituí-la.

**Site registrado nas conversas:** [Conta a Dois](https://conta-a-dois-marcus.nexoraconceito.chatgpt.site)

## Objetivo

Centralizar o controle financeiro individual e compartilhado, permitindo acompanhar despesas, meios de pagamento, parcelas, responsabilidades, pendências e acertos entre duas pessoas. O projeto também evoluiu para incluir uma carteira de recebimentos e um painel de alunos.

## Como rodar a recriação

Abra `index.html` no navegador. Os dados ficam no `localStorage` do próprio navegador (sem servidor). Use *Configurações → Exportar backup* para levar os dados a outro aparelho. Sincronização entre dois celulares, login, APK e push **não** existem nesta versão.

## Documentação

- [Visão geral e estado atual](docs/VISAO-GERAL.md)
- [Funcionalidades e módulos](docs/FUNCIONALIDADES.md)
- [Regras de negócio conhecidas](docs/REGRAS-DE-NEGOCIO.md)
- [Identidade visual e interface](docs/DESIGN-SYSTEM.md)
- [Arquitetura e integrações](docs/ARQUITETURA.md)
- [Roadmap e pendências](docs/ROADMAP.md)
- [Histórico de decisões](docs/HISTORICO.md)

## Estado conhecido

### Relatado como implementado no site
- Registro e acompanhamento de despesas individuais e compartilhadas.
- Identificação de despesas por pessoa e por meio de pagamento, incluindo cartão e Pix.
- Controle de compras parceladas.
- Acompanhamento de pendências e repasses entre as duas pessoas.
- Dados mantidos online no site.
- Módulo Carteira com painel de recebimentos.
- Painel de Alunos, mensalidades, pagamentos e outros ganhos.
- Ação para enviar mensagem pelo WhatsApp a partir do painel de alunos.
- Tabela compacta, com aparência de planilha/Excel, no painel de alunos.

### Planejado ou ainda não confirmado como concluído
- Acesso autônomo da segunda pessoa por convite/liberação.
- Aplicativo Android instalável/APK.
- Sincronização entre dois celulares Samsung.
- Notificações push configuráveis.
- Backend próprio e infraestrutura Firebase.
- Transformação em produto SaaS.

## Como contribuir

Antes de alterar funcionalidades, consulte as regras e o histórico documentados. Atualize esta documentação sempre que uma decisão de produto ou regra financeira mudar.

## Observação importante

Este repositório começou como base de documentação. Não contém, neste primeiro momento, uma cópia do código-fonte do site publicado, banco de dados, credenciais ou configuração de deploy. Não coloque segredos, tokens ou dados financeiros pessoais neste repositório.
