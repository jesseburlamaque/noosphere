---
noteId: "b8f2d0005a4511f18000d17e4ea03c9a"
tags: []

---

# Noosphere — Base de Conhecimento em Ciência Florestal, Clima e Geoespacial

> _A Noosfera, na visão de Teilhard de Chardin e Vernadsky, é a esfera do pensamento humano que emerge sobre a biosfera. Este vault é a minha camada pensante sobre a floresta._

## Filosofia

O Noosphere vault nasce da interseção entre ciência de ponta e organização pessoal do conhecimento. Cada nota é um nó em uma rede viva de conceitos — não um arquivo morto. O objetivo é simples: transformar uma pilha de PDFs esquecidos em um grafo de conhecimento navegável e acionável.

Três princípios:

1. **Atomicidade** — uma nota = um conceito. Papers viram notas atômicas no Inbox e são linkados a tópicos e projetos.
2. **Conexão primeiro** — o valor de uma nota está nas suas arestas. Todo paper novo deve se conectar a pelo menos um tópico existente.
3. **Processamento incremental** — inbox → processar → conectar. Nada de perfeccionismo. Um paper lido mas não linkado é melhor que um PDF esquecido.

## Estrutura de Pastas

```
Noosphere/
├── 00-Inbox/           # Captura inicial: papers recém-extraídos
├── 01-Papers/
│   ├── Processados/    # Papers lidos, anotados e linkados
│   └── Referencia/     # Papers de consulta rápida (não lidos na íntegra)
├── 02-Topicos/         # Notas de tópico temático
├── 03-Sinteses/         # Notas de síntese temática
├── 04-Projetos/        # Notas de projetos de pesquisa
├── 05-Templates/       # Templates para novas notas
└── 06-Meta/            # Documentação do próprio vault
    └── skills/         # Skills para assistentes de IA
```

## Workflow Resumido

```
📥 00-Inbox → captura automática (skill extrair-paper)
   ↓
🔍 Leitura e anotação → preencher crítica, ajustar tags
   ↓
🔗 Conexão → mover para 01-Papers/Processados/, linkar a tópicos
   ↓
🧹 Revisão semanal → auditar tags, conectar notas órfãs
```

Veja [[06-Meta/workflow]] para o passo a passo detalhado.

## Queries Dataview

### Papers não lidos (status = inbox)

```dataview
TABLE authors, year, journal AS "Periódico"
FROM "00-Inbox" OR "01-Papers"
WHERE status = "inbox"
SORT file.cday DESC
```

### Papers por tag de tópico

```dataview
TABLE authors, year, journal AS "Periódico"
FROM "01-Papers"
WHERE contains(tags, "#sensoriamento-remoto")
SORT year DESC
```

### Papers adicionados nos últimos 30 dias

```dataview
TABLE authors, year, status
FROM "00-Inbox" OR "01-Papers"
WHERE date(today) - file.cday <= dur(30 days)
SORT file.cday DESC
```

## Convenções de Tags

Use o arquivo [[06-Meta/tags]] como vocabulário controlado. Tags são organizadas em três grupos: **Status**, **Domínio** e **Output**. Mantenha a disciplina — tags demais matam o grafo.

---

_Última atualização: {{date}}_
