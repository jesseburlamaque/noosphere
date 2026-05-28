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

### 1. Renomear o PDF

Antes de extrair o conteúdo, renomeie o arquivo PDF seguindo o padrão:

```
Autor et al Ano - Título completo do paper.pdf
```

Regras:
- **Autor**: sobrenome do primeiro autor com capitalização normal (ex: `Araujo`, `Chave`, `Higuchi`)
- **et al**: se houver múltiplos autores
- **Ano**: ano de publicação
- **Título**: o título real completo do paper (extraído da primeira página do PDF), sem abreviações
- **Separação**: ` - ` (espaço, hífen, espaço) entre autor/ano e o título
- **Extensão**: sempre `.pdf`
- **Acentuação**: mantida (ex: `Dinâmica`, `São`)
- **Dois-pontos**: substituir por ` - ` (espaço, hífen, espaço)

Exemplos:
- `Chave et al 2014 - Improved allometric models to estimate the aboveground biomass of tropical trees.pdf`
- `Higuchi 2015 - Dinâmica de volume e biomassa da floresta de terra firme do Amazonas.pdf`
- `Silva 2007 - Alometria, estoque e dinâmica da biomassa de florestas primárias e secundárias na região de Manaus AM - Parte 1.pdf`

### 2. Leitura do PDF
- Leia o PDF completo antes de começar
- Priorize: abstract, introdução, conclusão, figuras e tabelas
- Se o PDF for escaneado e ilegível, avise o usuário

### 3. Extração do frontmatter
- `title`: título exato, sem abreviações
- `authors`: lista de sobrenomes + iniciais (ex: Silva J, Costa M)
- `year`: ano de publicação
- `doi`: se encontrado no PDF, senão deixe em branco
- `journal`: nome da revista ou conferência
- `tags`: selecione APENAS do vocabulário em `05-Meta/tags.md`
- `status`: sempre inicie como `inbox`

### 4. Preenchimento das seções

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

### 5. Nome do arquivo
Formato: `Autor et al Ano - palavras-chave-do-titulo.md`
Regras:
- **Autor**: sobrenome do primeiro autor capitalizado normalmente
- **et al**: se houver múltiplos autores (omitir se autor único)
- **Ano**: ano de publicação
- **Título**: 3-5 palavras-chave do título, minúsculas, separadas por hífen
- **Separador**: ` - ` entre autor/ano e o título

Exemplos:
- `Chave et al 2014 - improved-allometric-models-biomass.md`
- `Higuchi 2015 - dinamica-volume-biomassa-floresta.md`
- `Silva 2007 - alometria-estoque-dinamica-biomassa.md`

### 6. Salvar
Salve em `00-Inbox/`.
Confirme para o usuário: nome do arquivo criado + tags aplicadas.

### 7. Revisão de tags
Após salvar, verifique se todas as tags usadas existem em `05-Meta/tags.md`.
Se houver tags novas não documentadas, avise o usuário e aguarde confirmação
antes de qualquer alteração no vocabulário.
