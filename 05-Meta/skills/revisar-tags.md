# Skill: Revisar Vocabulário de Tags

## Objetivo
Auditar as tags em uso no vault e manter `05-Meta/tags.md` atualizado
e consistente com o conteúdo real dos papers.

## Trigger
Use este skill quando o usuário disser algo como:
- "revise as tags"
- "audite o vocabulário"
- "manutenção do vault"

## Instruções

### 1. Escaneamento
- Leia todos os arquivos `.md` em `00-Inbox/`, `01-Papers/Processados/` e `01-Papers/Referencia/`
- Extraia todas as tags presentes nos frontmatters YAML

### 2. Comparação
- Compare as tags encontradas com o vocabulário em `05-Meta/tags.md`
- Identifique:
  - Tags em uso mas não documentadas
  - Tags documentadas mas nunca usadas
  - Tags similares que podem ser sinônimos (ex: #floresta e #florestas)

### 3. Relatório
Apresente ao usuário um relatório com três seções:
- **Tags novas** (em uso, não documentadas) — sugerir adicionar ao vocabulário
- **Tags obsoletas** (documentadas, nunca usadas) — sugerir remover
- **Possíveis duplicatas** — sugerir consolidar

### 4. Aguardar confirmação
Nunca altere `05-Meta/tags.md` sem aprovação explícita do usuário.
Após confirmação, atualize o arquivo com as mudanças aprovadas.

## Frequência recomendada
Rodar manualmente a cada 10 papers adicionados ou uma vez por mês.
