# .agents

Comportamento Geral do Agente

Sempre seguir as diretrizes desse arquivo de instruções.

Leia todos os arquivos relevantes antes de fazer qualquer alteração
Nunca altere código fora do escopo explicitamente descrito na tarefa
Preserve todo o código existente que não está sendo modificado
Se encontrar ambiguidade ou risco de conflito, pergunte antes de implementar
Prefira editar arquivos existentes a criar novos sempre que possível
Nunca delete arquivos sem confirmação explícita do usuário

Qualidade de Código

Sempre use o mesmo padrão de código já existente no projeto (não mude style sem ser pedido)
Não adicione comentários desnecessários — comente apenas lógica não óbvia
Remova imports órfãos após qualquer refatoração
Não deixe console.log de debug no código final
Prefira funções pequenas e com responsabilidade única

Comunicação e Relatório

Ao finalizar qualquer tarefa, liste exatamente quais arquivos foram alterados e o que foi feito em cada um
Se encontrar um bug ou problema fora do escopo durante a implementação, reporte mas não corrija sem autorização
Use português para toda comunicação com o usuário
Sempre no final apresentar em formato de tabela os relatorios

Segurança

Nunca exponha secrets, tokens ou chaves de API no código
Nunca faça commit de arquivos .env
Sempre use variáveis de ambiente para dados sensíveis

Terminal

Antes de rodar qualquer comando destrutivo (delete, drop, reset), confirme com o usuário
Sempre rode o build/lint após alterações para garantir que não quebrou nada

Quando pedir para abrir um sistema que esta trabalhando, abrir o sistema logado e deixar que eu navegue.

Desenvolvimento

Sempre pegar o login e senha do banco que esta ativo para o sistema que esta trabalhando.

Não usar mock(mocado) nos código, sempre usar dados reais vindos da api`s integradas ao banco.

Realizar desenvolvimento, sempre desenvolver front, api e banco.

Eu decido quando tem que atualizar o repositorio no git.

Sempre conversar comigo em pt-br

Sempre no final de algum desenvolvimento, se houver alterações/inclusão no banco de dados , atualizar/gerar scripts no projeto banco.

Não utilize o modo visual ou capturas de tela (screenshots) para ler o código. Foque apenas na leitura direta dos arquivos de texto e logs do terminal para economizar tempo.





<!-- context7 -->

Use Context7 MCP to fetch current documentation whenever the user asks about a library, framework, SDK, API, CLI tool, or cloud service -- even well-known ones like React, Next.js, Prisma, Express, Tailwind, Django, or Spring Boot. This includes API syntax, configuration, version migration, library-specific debugging, setup instructions, and CLI tool usage. Use even when you think you know the answer -- your training data may not reflect recent changes. Prefer this over web search for library docs.

Do not use for: refactoring, writing scripts from scratch, debugging business logic, code review, or general programming concepts.

## Steps

1. Always start with `resolve-library-id` using the library name and the user's question, unless the user provides an exact library ID in `/org/project` format
2. Pick the best match (ID format: `/org/project`) by: exact name match, description relevance, code snippet count, source reputation (High/Medium preferred), and benchmark score (higher is better). If results don't look right, try alternate names or queries (e.g., "next.js" not "nextjs", or rephrase the question). Use version-specific IDs when the user mentions a version
3. `query-docs` with the selected library ID and the user's full question (not single words)
4. Answer using the fetched docs

<!-- context7 -->

