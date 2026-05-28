---
noteId: "b2e436e05a4511f18000d17e4ea03c9a"
tags: []
aliases: null
created:
  [object Object]: null

---

# {{title}}

## Definição

{{definicao}}

## Papers-chave

```dataview
TABLE authors, year, journal
FROM "01-Papers"
WHERE contains(tags, this.file.tags[0])
SORT year DESC
```

## Perguntas em aberto

- {{pergunta1}}
- {{pergunta2}}
- {{pergunta3}}

## Projetos relacionados

```dataview
LIST
FROM "04-Projetos"
WHERE contains(file.outlinks, this.file.link)
```
