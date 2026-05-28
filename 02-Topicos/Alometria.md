---
noteId: "alometria-topico"
tags:
  - alometria
aliases:
  - "Alometria"
  - "Relação DAP-altura-volume"
  - "Modelos alométricos"
---

# Alometria

## Definição

Relações matemáticas entre dimensões mensuráveis das árvores (DAP, altura, densidade da madeira) e sua biomassa. Modelos alométricos são a principal ferramenta para estimar estoques de biomassa e carbono em florestas tropicais, podendo ser regionais (calibrados para um sítio específico) ou pan-tropicais (genéricos para todos os biomas tropicais).

## Papers-chave

```dataview
TABLE authors, year, journal
FROM "00-Inbox" OR "01-Papers"
WHERE contains(tags, "#alometria")
SORT year DESC
```

## Perguntas em aberto

- Até que ponto a variação regional na relação DAP-altura invalida modelos pan-tropicais?
- Qual a contribuição relativa de modelos específicos para raízes grossas vs. equações de parte aérea na redução da incerteza total do estoque de carbono?
- Como incorporar florestas secundárias (capoeiras) em modelos pan-tropicais existentes?

## Projetos relacionados

```dataview
LIST
FROM "04-Projetos"
WHERE contains(file.outlinks, this.file.link)
```
