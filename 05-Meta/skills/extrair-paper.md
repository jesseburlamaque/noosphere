# Skill: Extrair Paper para Nota Obsidian

## Objetivo
Ler um PDF científico e gerar automaticamente uma nota Markdown preenchida,
compatível com o vault Noosphere, salva em `00-Inbox/`.

## Trigger
Use este skill quando o usuário disser algo como:
- "extraia este paper"
- "processe este PDF"
- "adicione ao vault"

## Instruções

### 1. Leitura do PDF
- Leia o PDF completo antes de começar
- Priorize: abstract, introdução, conclusão, figuras e tabelas
- Se o PDF for escaneado e ilegível, avise o usuário

### 2. Extração do frontmatter
- `title`: título exato, sem abreviações
- `authors`: lista de sobrenomes + iniciais (ex: Silva J, Costa M)
- `year`: ano de publicação
- `doi`: se encontrado no PDF, senão deixe em branco
- `journal`: nome da revista ou conferência
- `tags`: selecione APENAS do vocabulário em `05-Meta/tags.md`
- `status`: sempre inicie como `inbox`

### 3. Preenchimento das seções

**Resumo em uma frase**
Uma única frase que responda: "Este paper mostra que..."
Seja específico — evite frases genéricas.

**Problema que resolve**
2-3 frases sobre a lacuna de conhecimento ou problema aplicado.

**Principais achados**
3 a 5 bullet points com resultados importantes.
Inclua números e métricas quando disponíveis.

**Metodologia**
3-5 frases: área de estudo, dados utilizados, métodos, período temporal.

**Minha crítica**
Deixe sempre com o placeholder: `_a preencher_`
Nunca invente uma opinião pelo usuário.

**Conexões com outras notas**
- Verifique arquivos `.md` em `01-Papers/` e `02-Topicos/`
- Sugira links no formato `[[nome-da-nota]]` apenas se houver relação clara
- Se o vault estiver vazio: `_nenhuma conexão identificada ainda_`

### 4. Nome do arquivo
Formato: `YYYY-SOBRENOME-palavra-chave-do-titulo.md`
Exemplo: `2023-SILVA-desmatamento-amazonia.md`

### 5. Salvar
Salve em `00-Inbox/`.
Confirme para o usuário: nome do arquivo criado + tags aplicadas.

### 6. Revisão de tags
Após salvar, verifique se todas as tags usadas existem em `05-Meta/tags.md`.
Se houver tags novas não documentadas, avise o usuário e aguarde confirmação
antes de qualquer alteração no vocabulário.
