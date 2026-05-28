---
noteId: "c20f6c705a4511f18000d17e4ea03c9a"
tags: []

---

# Workflow Noosphere

## 1. Capturar (5 min)

**Quando:** encontrou um paper interessante.
**Onde:** `00-Inbox/`

1. Use a skill [[05-Meta/skills/extrair-paper]] para gerar a nota automaticamente
2. Ou crie manualmente usando o template `04-Templates/nota-paper.md`
3. A nota nasce com `status: inbox`

**Regra:** quantidade > qualidade na captura. Se parecer relevante, entra. Decide-se depois.

## 2. Processar (30-60 min)

**Quando:** reservou tempo para leitura focada.
**Onde:** `00-Inbox/` → `01-Papers/Processados/` (após concluir)

1. Leia o PDF com a nota aberta ao lado
2. Atualize o resumo em uma frase
3. Preencha **Minha crítica** — sem isso, o paper não está processado
4. Ajuste as tags: remova `#inbox`, adicione `#concluido` e tags de domínio
5. Mude `status` para `concluido`
6. Mova o PDF (se houver) para `01-Papers/Processados/`

**Regra:** a crítica é o que separa uma anotação de uma coleção. Seja sincero, não reverente.

## 3. Conectar (10 min)

**Quando:** imediatamente após processar.

1. Crie ou atualize notas em `02-Topicos/` que se relacionem com o paper
2. Adicione `[[wiki-links]]` na seção "Conexões com outras notas"
3. Se o paper merece destaque, taggeie como `#achado-chave` ou `#para-citar`

**Regra:** um paper sem links é um paper órfão. Todo paper precisa de ≥1 link para um tópico.

## 4. Revisão Semanal (30 min)

**Quando:** toda sexta-feira.

1. **Inbox zero:** processe ou mova para `01-Papers/Referencia/` tudo que está em `00-Inbox/`
2. **Auditoria de tags:** rode a skill [[05-Meta/skills/revisar-tags]]
3. **Notas órfãs:** verifique papers sem links de saída
4. **Dataview:** cheque a query de papers não lidos — se passou 30 dias em `#inbox`, mova para `01-Papers/Referencia/`

## Atalhos

- **Paper de consulta rápida:** crie nota com `status: referencia` e mova direto para `01-Papers/Referencia/` — sem crítica, sem conexão.
- **Paper próprio (autor):** regras normais se aplicam. Crítica é _mais_ importante.
