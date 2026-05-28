---
noteId: "biomassa-topico"
tags:
  - "biomassa"
aliases:
  - "Biomassa florestal"
  - "Estoque de biomassa"
  - "Biomassa acima do solo"
  - "Biomassa abaixo do solo"
---

# Biomassa

## Definição

Massa total de matéria orgânica viva (tronco, galhos, folhas, raízes) em um ecossistema florestal, geralmente expressa em Mg ha⁻¹ ou t ha⁻¹. A biomassa acima do solo (AGB/AGW) inclui tronco, galhos e folhas; a biomassa abaixo do solo (BGB/BGW) inclui raízes grossas e finas. É o principal componente para estimativas de estoque de carbono florestal (≈ 48-50% da biomassa seca é carbono).

## Papers-chave

```dataview
TABLE authors, year, journal
FROM "00-Inbox" OR "01-Papers"
WHERE contains(tags, "#biomassa")
SORT year DESC
```

## Perguntas em aberto

- Qual a contribuição de raízes finas (< 2 mm) no estoque total de biomassa abaixo do solo?
- Como a biomassa de florestas secundárias se compara à de florestas primárias em diferentes idades de regeneração?
- A razão parte aérea:raízes é consistente entre diferentes tipos de solo e gradientes climáticos na Amazônia?

## Projetos relacionados

```dataview
LIST
FROM "04-Projetos"
WHERE contains(file.outlinks, this.file.link)
```
