---
noteId: "sintese-biomassa-alometria"
tags:
  - "biomassa"
  - "amazonia"
  - "metodologia"
---

# Síntese - Estoques de biomassa e modelos alométricos na Amazônia

Os quatro papers convergem para a necessidade de modelos alométricos calibrados regionalmente na Amazônia, mas divergem sobre a generalizabilidade de equações pan-tropicais, com estimativas de biomassa total variando de 252,6 Mg.ha⁻¹ (Rio Negro) a 339,8 t.ha⁻¹ (média do Amazonas), dependendo da região e do método.

## Papers consultados

- [[Chave et al 2014 - improved-allometric-models-biomass-pantropical]]
- [[Lima et al 2012 - allometric-models-biomass-above-below-ground-rio-negro]]
- [[Silva 2007 - allometry-stock-dynamics-biomass-manaus]]
- [[Higuchi 2015 - volume-biomass-carbon-dynamics-amazonas]]

## Variáveis comparadas

| Variável | Chave et al 2014 | Lima et al 2012 | Silva 2007 | Higuchi 2015 |
|----------|-----------------|-----------------|-----------|--------------|
| Região | Pantropical (58 sítios) | Alto Rio Negro (NW) | Manaus (Central) | Amazonas (11 locais) |
| Tipo de floresta | Todas as formações tropicais | Terra firme primária | Primária + capoeira | Terra firme primária |
| n amostral | 4004 árvores (58 sítios) | 101 árvores (2 parcelas) | 494 aérea + 131 raízes | 1128 parcelas (295,5 ha) |
| DAP mínimo | 5 cm | 5 cm | 10 cm | 10 cm |
| Equação principal | ln(AGB) = -2,024 + 2,307 ln(D) + 0,595 ln(ρ) + 0,649 ln(H) | ln(AGW) = -2,025 + 2,459 ln(D) | PF = 2,7179 × DAP^1,8774 | Silva (2007) corrigida por Hdom |
| Densidade da madeira (ρ) | Sim — preditor essencial | Não | Não | Não |
| Biomassa subterrânea | Não | Sim — BGW = 0,136 × AGW | Sim — 27,1% da biomassa viva | Sim (raízes grossas via Silva 2007) |
| Biomassa total (Mg.ha⁻¹) | — | 252,6 | — | 339,8 ± 25,4 |
| Carbono total (t.ha⁻¹) | — | — | — | 164,8 ± 12,3 |
| Erro/Precisão | ~56% por árvore; ~10% em 1 ha | R² = 0,944 (AGW) | r² = 0,94 (simples); 0,95 (dupla) | IC < 10% para todas as estimativas |
| Posição sobre modelo único | Defende modelo pan-tropical único | Evidencia diferenças regionais (p < 0,05) | Modelos regionais para Manaus | ANCOVA rejeita equação única (p < 0,000001) |

## Análise por paper

### [[Chave et al 2014 - improved-allometric-models-biomass-pantropical]]

- Propõe e valida um modelo pan-tropical único usando DAP, densidade da madeira (ρ) e altura total (H) — Eq. 4: ln(AGB) = -2,024 + 2,307 ln(D) + 0,595 ln(ρ) + 0,649 ln(H)
- Quando altura não está disponível, propõe substituí-la por uma variável bioclimática composta E (deficit hídrico + sazonalidade) — Eq. 7
- Conclui que um único modelo serve para todas as formações tropicais, sem efeito significativo de região ou bioma
- Erro médio de ~56,5% por árvore, caindo para ~10% em parcelas de 1 ha
- Densidade da madeira é preditor essencial: modelos sem ρ tiveram AIC 3983 vs. 3855 com ρ
- Seis sítios (florestas úmidas) fogem do padrão geral, sugerindo que árvores com sapopemas ou medições históricas podem introduzir viés

### [[Lima et al 2012 - allometric-models-biomass-above-below-ground-rio-negro]]

- Desenvolve modelos alométricos específicos para o noroeste da Amazônia (São Gabriel da Cachoeira, alto Rio Negro)
- Melhor modelo para biomassa aérea: ln(AGW) = -2,025 + 2,459 ln(D), R² = 0,944
- Biomassa subterrânea segue relação constante: BGW = 0,136 × AGW, independente do tamanho da árvore
- Biomassa total estimada: 252,6 Mg.ha⁻¹ (222,2 aérea + 30,7 subterrânea) — valor 73% menor que meta-análises anteriores (~380–400 Mg.ha⁻¹)
- ANCOVA mostra que a relação D-AGW difere significativamente entre Leste, Centro, Sul e Noroeste da Amazônia (p < 0,05)
- Altura assintótica de 33,4 m, menor que na Amazônia central (41,4 m) e oriental (73,0 m)

### [[Silva 2007 - allometry-stock-dynamics-biomass-manaus]]

- Desenvolve modelos alométricos para Manaus (ZF-2) incluindo biomassa aérea e raízes grossas
- Modelo de simples entrada: PF = 2,7179 × DAP^1,8774 (r² = 0,94); dupla entrada: PF = 0,5521 × DAP^1,6629 × HT^0,7224 (r² = 0,95)
- Teor de água: 41,6%; teor de carbono: 48,5%
- Biomassa viva = 97,1% do total; raízes grossas = 27,1% da biomassa viva
- Capoeira de 14 anos: incremento de 10,8 t.ha⁻¹.ano⁻¹; capoeira de 23 anos: 10,6 t.ha⁻¹.ano⁻¹
- Custo médio por árvore para biomassa total: R$ 805 ± 310 (IC 95%); 100 árvores suficientes para erro < 10%

### [[Higuchi 2015 - volume-biomass-carbon-dynamics-amazonas]]

- Inventário florestal contínuo em escala estadual (11 localidades, 1128 parcelas, 295,5 ha)
- Volume comercial médio (DAP ≥ 50 cm): 20,3 ± 5,3 m³.ha⁻¹
- Carbono total médio (acima do solo + raízes grossas, DAP ≥ 10 cm): 164,8 ± 12,3 t.ha⁻¹ (IC 95%)
- Biomassa seca total: 339,8 ± 25,4 t.ha⁻¹
- Usa equação de Silva (2007) como base, corrigida por fator de altura dominante (Hdom) — Hdom de cada sítio dividida pela Hdom de Manaus (30,2 m)
- ANCOVA rejeita equação de volume única para o estado (p < 0,000001 em todos os sítios)
- Erro amostral < 10% para todas as estimativas — o menor IC foi 2,5% (Flona de Pau Rosa)

## Conclusões da síntese

1. **A necessidade de modelos regionais é consistente entre os três estudos amazônicos.** Lima (2012), Silva (2007) e Higuchi (2015) encontraram diferenças significativas nas relações alométricas entre regiões da Amazônia, corroborando a rejeição de um modelo único — tanto Chave (2014) quanto Higuchi (2015) reportam testes estatísticos que apontam na mesma direção (p < 0,05 e p < 0,000001, respectivamente).

2. **Chave et al (2014) é o único que defende um modelo pan-tropical único**, mas seus próprios dados mostram que 6 dos 58 sítios fogem do padrão geral, e os sítios amazônicos contribuíram com parte relevante da variação residual (78% explicada pelo sítio, 0,6% pela densidade da madeira). Isso sugere que o modelo pan-tropical funciona bem em escala global (~10% de erro por hectare), mas modelos regionais reduzem o erro em contextos específicos.

3. **As estimativas de biomassa total variam substancialmente entre regiões amazônicas.** Lima (2012) encontrou 252,6 Mg.ha⁻¹ no Rio Negro (NW), enquanto Higuchi (2015) estimou 339,8 t.ha⁻¹ como média do Amazonas — diferença de ~35%. Esta variação é consistente com gradientes de altura (Hdom) e fertilidade do solo documentados em ambos os estudos.

4. **A altura dominante (Hdom) é um preditor crítico para transferibilidade de modelos.** Higuchi (2015) desenvolveu um fator de correção baseado em Hdom que permite adaptar a equação de Silva (2007) para outros sítios, e Lima (2012) confirmou que diferenças na relação D-H explicam as diferenças regionais nos modelos.

5. **A densidade da madeira é subutilizada nos estudos amazônicos.** Apenas Chave (2014) inclui ρ como preditor, demonstrando que sua exclusão aumenta o erro. Nenhum dos três estudos amazônicos incorporou ρ em seus modelos, o que representa uma oportunidade de melhoria.

6. **Os níveis de incerteza são raramente reportados de forma comparável.** Chave (2014) reporta erro por árvore e por hectare; Silva (2007) reporta r² e erro padrão; Lima (2012) reporta R² e Syx; Higuchi (2015) reporta IC 95% amostral. A falta de padronização dificulta a comparação direta da precisão entre os estudos.

## Perguntas em aberto

- A inclusão de densidade da madeira (ρ) nos modelos regionais amazônicos reduziria significativamente a incerteza das estimativas, a ponto de tornar os modelos regionais equivalentes ao modelo pan-tropical?
- O fator de correção por Hdom proposto por Higuchi (2015) pode ser generalizado para outras regiões da Amazônia além do Amazonas?
- Qual a contribuição relativa da biomassa subterrânea em diferentes tipos de solo e formações florestais na Amazônia — a relação constante BGW/AGW de 0,136 (Lima, 2012) se mantém em outras regiões?
