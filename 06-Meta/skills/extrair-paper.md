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
- `doi`: link clicável completo (`https://doi.org/10...`) se encontrado no PDF; se não houver DOI, deixe em branco (`""`) para preenchimento manual
- `journal`: nome da revista ou conferência
- `tags`: selecione APENAS do vocabulário em `06-Meta/tags.md`
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

1. **Varra `02-Topicos/`** — para cada nota de tópico existente, verifique se o paper se relaciona com o tema. Em caso positivo, adicione `[[topico]]` + uma frase curta explicando a relação.
2. **Varra `00-Inbox/` e `01-Papers/`** — se outro paper tratar de tema, região ou método similar, adicione `[[autor et al ano - keywords-regiao]]` + explicação da relação.
3. **Identifique lacunas** — se um conceito central do paper (ex: "alometria", "biomassa", "carbono") não tiver nota de tópico correspondente, anote mentalmente para criar na etapa 6.
4. **Se o vault estiver vazio** (primeiro paper): `_nenhuma conexão identificada ainda_`

### 5. Nome do arquivo
Formato: `Autor et al Ano - keyword1-keyword2-keyword3-regiao.md`
Regras:
- **Autor**: sobrenome do primeiro autor capitalizado normalmente
- **et al**: se houver múltiplos autores (omitir se autor único)
- **Ano**: ano de publicação
- **Keywords**: 3-5 palavras-chave em **inglês** (minúsculas, separadas por hífen), extraídas do título ou do tema central do paper
- **Região**: última palavra do nome, indicando a região geográfica do estudo (ex: `pantropical`, `amazonia-central`, `rio-negro`, `manaus`, `peru`)
- **Separador**: ` - ` entre autor/ano e as keywords

Exemplos:
- `Chave et al 2014 - improved-allometric-models-biomass-pantropical.md`
- `Higuchi 2015 - dinamica-volume-biomassa-floresta.md`
- `Lima et al 2012 - allometric-models-biomass-above-below-ground-rio-negro.md`
- `Silva 2007 - allometry-stock-dynamics-biomass-manaus.md`

### 6. Criação de notas de tópico

Se na etapa 4 você identificou um conceito central sem nota de tópico correspondente em `02-Topicos/`:

1. **Crie a nota** em `02-Topicos/` usando como referência o template `05-Templates/nota-topico.md`
2. **Definição**: 2-4 frases explicando o conceito
3. **Papers-chave**: o Dataview consultará as tags automaticamente; adicione também a tag correta no frontmatter da nota de tópico
4. **Perguntas em aberto**: 2-3 perguntas derivadas do paper recém-lido e da literatura
5. **Adicione `[[novo-paper]]`** na seção "Conexões com outras notas" do paper criado
6. **Confirme** com o usuário: "Nota de tópico [nome] criada em 02-Topicos/"

### 7. Salvar
Salve em `00-Inbox/`.
Confirme para o usuário: nome do arquivo criado + tags aplicadas.

### 8. Revisão de tags
Após salvar, verifique se todas as tags usadas existem em `06-Meta/tags.md`.
Se houver tags novas não documentadas, avise o usuário e aguarde confirmação
antes de qualquer alteração no vocabulário.
