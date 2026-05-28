---
noteId: "graph-config"
tags: []
---

# Configuração do Grafo

## Grupos de cor recomendados

Os grupos já estão configurados em `.obsidian/graph.json`. Para ajustar manualmente:

Obsidian → Graph View → ⚙️ (gear icon, canto superior direito) → **Groups**.

O painel "Groups" aparece na parte inferior das configurações do grafo. Clique em **New group** e defina:

| Grupo | Query | Cor |
|-------|-------|-----|
| Inbox | `path:00-Inbox` | Azul |
| Papers | `path:01-Papers` | Verde |
| Sínteses | `path:03-Sinteses` | Roxo |
| Tópicos | `path:02-Topicos` | Laranja |
| Meta | `path:06-Meta` | Cinza |

## Forças (Display)

Ajuste em Graph View → ⚙️ → Display:

- **Distance between nodes**: 120–150 (diminui para clusters mais densos)
- **Neighborhood**: 60.000 (maior = conexões mais visíveis)
- **Repulsion**: 8.000–10.000 (menor = nós mais agregados)
- **Central Attraction**: 0.05–0.10 (maior = grafo mais compacto)

## Filtros úteis

- **Orphans ON** — destaca notas sem nenhum link (boas para auditoria)
- **Tags OFF** — evita que tags criem nós gigantes que distorcem o grafo
- **Attachments OFF** — oculta imagens/anexos não relevantes
