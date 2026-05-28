---
noteId: "amazonia-central-topico"
tags:
  - "amazonia-central"
aliases:
  - "Amazônia Central"
  - "Região de Manaus"
  - "ZF-2"
  - "BR-174"
---

# Amazônia Central

## Definição

Região da Amazônia brasileira centrada em Manaus (AM), compreendendo a Estação Experimental de Silvicultura Tropical do INPA (ZF-2, km 50 da BR-174) e áreas adjacentes. Caracteriza-se por florestas de terra firme sobre platôs e baixios, com dossel entre 30-40 m e altura assintótica em torno de 41 m. É a região mais amostrada para estudos de biomassa e alometria na Amazônia brasileira.

## Papers-chave

```dataview
TABLE authors, year, journal
FROM "00-Inbox" OR "01-Papers"
WHERE contains(tags, "#amazonia-central" OR "#manaus")
SORT year DESC
```

## Perguntas em aberto

- Como os modelos alométricos da Amazônia central se comportam quando aplicados a outras regiões (oriental, sul, noroeste)?
- A dinâmica de biomassa em florestas de platô vs. baixio difere em resposta a eventos de seca extrema?
- Qual o papel das florestas secundárias na paisagem da Amazônia central para o balanço regional de carbono?

## Projetos relacionados

```dataview
LIST
FROM "04-Projetos"
WHERE contains(file.outlinks, this.file.link)
```
