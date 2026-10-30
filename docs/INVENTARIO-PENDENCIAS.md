# Inventário de Evidências e Pendências

Este documento impede que conhecimento parcial seja confundido com implementação comprovada.

## Fontes conhecidas

- Conversas do projeto recuperadas até 30/10/2026.
- Site publicado registrado: https://conta-a-dois-marcus.nexoraconceito.chatgpt.site
- Repositório GitHub: https://github.com/Animehall/conta-a-dois

A URL publicada não foi acessível pela ferramenta de inspeção nesta etapa. Portanto, nenhuma estrutura interna, tecnologia, tela ou banco foi inferido a partir dela.

## Funcionalidades relatadas como existentes

| Item | Evidência disponível | Estado |
|---|---|---|
| Despesas individuais e compartilhadas | Relato de 20/10/2026 | Relatado; verificar no código |
| Pessoa e meio de pagamento por despesa | Relato de 20/10/2026 | Relatado; verificar no código |
| Cartão e Pix | Relato de 20/10/2026 | Relatado; verificar no código |
| Compras parceladas | Relato de 20/10/2026 | Relatado; verificar no código |
| Pendências e repasses | Relato de 20/10/2026 | Relatado; verificar no código |
| Dados online no site | Relato de 20/10/2026 | Relatado; identificar backend |
| Dashboard de recebimentos na Carteira | Relato de 21/10/2026 | Relatado; verificar no código |
| Painel de Alunos e mensalidades | Relato de 21/10/2026 | Relatado; verificar no código |
| Pagamentos e outros ganhos | Relato de 21/10/2026 | Relatado; verificar no código |
| Ação de WhatsApp | Relato de 21/10/2026 | Relatado; verificar fluxo |
| Tabela compacta tipo Excel | Relato de 21/10/2026 | Relatado; verificar interface |

## Objetivos ainda não confirmados como concluídos

- Convite e acesso independente da segunda pessoa.
- APK/aplicativo Android.
- Sincronização entre dois celulares Samsung.
- Notificações push.
- Backend próprio/Firebase.
- Produto SaaS.

## Lacunas técnicas

| Área | O que precisa ser descoberto |
|---|---|
| Código-fonte | Linguagem, framework, estrutura de pastas, dependências |
| Interface | Todas as páginas, menus, modais, formulários, estados vazios e responsividade |
| Design | Cores, tipografia, espaçamentos, ícones, componentes e estados |
| Dados | Entidades, campos, relacionamentos, histórico e regras de exclusão |
| Autenticação | Como usuários entram, sessões e recuperação de acesso |
| Permissões | O que cada participante pode ver e editar |
| Financeiro | Fórmulas reais de divisão, parcelas, pendências e repasses |
| Integrações | WhatsApp, pagamentos, serviços externos |
| Infraestrutura | Hospedagem, domínio, backend, banco, armazenamento |
| Qualidade | Testes, logs, tratamento de erros e backups |
| Entrega | Build, deploy, domínio, APK e pipeline |

## Materiais necessários para completar o inventário

1. Exportação/ZIP do código-fonte original, se disponível.
2. Capturas de tela ou gravação navegando por todas as áreas do site.
3. Esquema do banco de dados ou exportação sem dados pessoais reais.
4. Lista de integrações e serviços usados.
5. Arquivo de configuração de exemplo, sem segredos.
6. Regras financeiras que ainda não estejam explícitas.

## Segurança ao compartilhar materiais

Antes de enviar arquivos:
- remover `.env` real, tokens, senhas e chaves privadas;
- remover dados financeiros pessoais e identificadores sensíveis;
- substituir registros reais por dados fictícios;
- nunca compartilhar credenciais de acesso ao painel de hospedagem.

## Critério de conclusão do inventário

O inventário só será considerado completo quando cada página e fluxo tiver:
- evidência visual ou código correspondente;
- comportamento descrito;
- dados de entrada e saída identificados;
- regras de validação documentadas;
- estados de erro e vazio descritos;
- testes ou passos de verificação registrados.
