---
noteId: "b8275d805aa411f1896a99c75c1c3e54"
tags: []

---

# Skill: Sintetizar Papers

## Objetivo
Cruzar dados de múltiplos papers para gerar uma nota de síntese com tabelas comparativas, análises por paper e conclusões baseadas exclusivamente em evidências dos PDFs originais.

## Trigger
Use este skill quando o usuário disser algo como:
- "cruze os dados de [papers]"
- "faça uma síntese de [papers]"
- "compare [paper A] com [paper B]"
- "compile as informações sobre [tema]"
- "o que os papers dizem sobre [variável]"

## Instruções

### 1. Identificar os papers alvo

O usuário pode especificar quais papers sintetizar de duas formas:

**Por nome**: "sintetize Chave 2014 e Higuchi 2015"
- Leia as notas em `00-Inbox/` e `01-Papers/` correspondentes

**Por tema/tag**: "síntese sobre biomassa na Amazônia central"
- Varra `00-Inbox/` e `01-Papers/` filtrando por tags (ex: `#biomassa` + `#amazonia-central`)
- Liste os papers encontrados e peça confirmação ao usuário

### 2. Validar dados nos PDFs originais

Para cada paper identificado:

1. **Localize o PDF** correspondente em `_pdfs/` pelo nome do arquivo (padrão: `Autor et al Ano - Título.pdf`)
2. **Extraia o texto** do PDF e releia as seções relevantes (abstract, resultados, tabelas, conclusão)
3. **Confronte** cada número, métrica ou afirmação da nota `.md` com o PDF original
4. Se houver divergência, **prevalece o PDF original** — corrija a nota se necessário e documente a correção

### 3. Estruturar a síntese

Crie a nota seguindo o template `04-Templates/nota-sintese.md`:

**Título**: `Síntese - [tema central].md`
Salve em `02-Topicos/` (ex: `02-Topicos/Síntese - Modelos Alométricos na Amazônia.md`)

**Resumo em uma frase**: Uma frase que sintetize o que o conjunto dos papers revela.

**Papers consultados**: Lista de `[[wikilinks]]` para cada papel incluído.

**Variáveis comparadas**: Tabela Markdown. Selecione variáveis que sejam diretamente comparáveis entre os papers (ex: estoque de carbono, equação alométrica, R², n amostral, região). Se os papers medirem grandezas diferentes, indique na coluna "Observação".

**Análise por paper**: Para cada paper, 3-5 bullet points com:
- O que o paper mediu ou estimou
- Como mediu (método resumido)
- Resultados principais (com valores exatos do PDF)
- Limitações declaradas pelo próprio autor

**Conclusões da síntese**: Apenas afirmações que:
- São suportadas por dados em pelo menos um dos papers
- Têm o paper citado entre parênteses — ex: `(Chave et al 2014)`
- Quando houver discordância entre papers, explicite o conflito — ex: "Chave et al 2014 defende que... enquanto Higuchi 2015 encontrou..."

**Perguntas em aberto**: Lacunas que persistem após a comparação.

### 4. Regras de evidência

- **Nunca invente números.** Todo valor numérico deve ter origem explícita (paper + seção ou tabela)
- **Nunca suavize contradições.** Se dois papers chegam a conclusões opostas, apresente ambas com seus respectivos dados
- **Contextualize diferenças** — se dois valores diferem, aponte possíveis causas (região diferente, método diferente, n amostral, ano)
- **Cite sempre** no formato: `(Autor et al, ano)` ou `(Autor, ano)`

### 5. Salvar e confirmar

Salve em `02-Topicos/`.
Confirme para o usuário: nome da síntese criada + papers incluídos + variáveis comparadas + número de conclusões.
