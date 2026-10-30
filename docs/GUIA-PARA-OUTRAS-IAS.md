# Guia de Continuidade para Outras IAs

Este arquivo é o ponto de entrada para qualquer IA que vá trabalhar no Conta a Dois.

## Missão

Continuar o desenvolvimento do Conta a Dois sem perder sua finalidade, regras conhecidas, decisões e histórico. O GitHub é a fonte central de documentação e código versionado do projeto.

## Antes de começar

Leia nesta ordem:
1. `README.md`
2. `docs/ESSENCIA-DO-PRODUTO.md`
3. `docs/VISAO-GERAL.md`
4. `docs/FUNCIONALIDADES.md`
5. `docs/REGRAS-DE-NEGOCIO.md`
6. `docs/DESIGN-SYSTEM.md`
7. `docs/ARQUITETURA.md`
8. `docs/ROADMAP.md`
9. `docs/HISTORICO.md`
10. `docs/INVENTARIO-PENDENCIAS.md`

## Contexto essencial

Conta a Dois é um produto de organização financeira individual e compartilhada. Deve ajudar duas pessoas a entender despesas, pagamentos, parcelas, responsabilidades, pendências e repasses. A divisão padrão conhecida para despesas compartilhadas é 50/50, mas despesas individuais devem continuar individuais.

Também foram relatados módulos Carteira e Painel de Alunos, com recebimentos, mensalidades, outros ganhos e contato por WhatsApp. A integração desses módulos com o núcleo financeiro ainda precisa ser inspecionada.

Site publicado registrado no histórico:
https://conta-a-dois-marcus.nexoraconceito.chatgpt.site

Repositório:
https://github.com/Animehall/conta-a-dois

## Regras de trabalho

- Não recriar o projeto do zero antes de inspecionar o código existente.
- Não substituir tecnologias ou arquitetura apenas por preferência.
- Não remover funcionalidades para simplificar sem autorização.
- Não alterar regras de divisão, parcelas, saldos ou repasses sem validar o impacto.
- Não afirmar que Firebase, APK, push ou sincronização entre dois celulares estão prontos: eram objetivos ainda não confirmados.
- Não assumir que o site publicado revela o código-fonte.
- Não colocar segredos, tokens, credenciais, dados bancários ou dados pessoais reais no Git.
- Usar variáveis de ambiente e fornecer um `.env.example` sem valores secretos, quando houver código.
- Criar commits pequenos e descritivos.
- Atualizar os documentos afetados em cada mudança.

## Protocolo para uma tarefa

1. Explique em uma frase o comportamento atual que encontrou.
2. Identifique arquivos e módulos afetados.
3. Verifique dependências e efeitos sobre cálculos financeiros.
4. Implemente a menor mudança segura.
5. Execute testes, lint e build disponíveis.
6. Informe arquivos alterados, testes executados e limitações.
7. Atualize documentação e histórico.

## Prioridades de qualidade

- Integridade dos valores monetários.
- Consistência entre dashboard, tabelas e detalhes.
- Responsividade para celular e desktop.
- Acessibilidade de formulários e ações.
- Sincronização segura e tratamento de conflitos.
- Autorização por participante.
- Backup, recuperação e rastreabilidade.

## Como lidar com informação desconhecida

Marque cada item como:
- **Confirmado:** existe evidência no código, teste ou observação verificável.
- **Relatado:** foi descrito em conversas, mas ainda não foi inspecionado.
- **Planejado:** objetivo futuro.
- **A validar:** regra ou comportamento ambíguo.

Nunca transforme um item relatado ou planejado em confirmado sem evidência.

## Primeira tarefa recomendada

Recuperar e importar o código-fonte original do site publicado, preservando uma cópia de segurança. Em seguida:
- mapear páginas, componentes e fluxos;
- identificar banco de dados, autenticação e integrações;
- documentar variáveis de ambiente sem expor segredos;
- executar o projeto localmente;
- comparar a versão local com o site publicado;
- só então planejar refatorações e evolução Android.
