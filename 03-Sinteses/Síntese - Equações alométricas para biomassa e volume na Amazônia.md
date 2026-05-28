---
noteId: sintese-equacoes-alometricas
tags:
  - alometria
  - biomassa
  - amazonia
---

# Síntese - Equações alométricas para biomassa e volume na Amazônia

## Resumo em uma frase

Os seis papers fornecem mais de 30 equações alométricas documentadas, abrangendo desde modelos pan-tropicais com 4004 árvores (Chave et al., 2014) até equações de volume específicas por sítio com 62–219 árvores cada (Higuchi, 2015), com R² variando de 0,85 a 0,97 e erro padrão de 1,8% a 15,17%.

## Papers consultados

- [[Chave et al 2014 - improved-allometric-models-biomass-pantropical]]
- [[Lima et al 2012 - allometric-models-biomass-above-below-ground-rio-negro]]
- [[Silva 2007 - allometry-stock-dynamics-biomass-manaus]]
- [[Higuchi 2015 - volume-biomass-carbon-dynamics-amazonas]]
- [[Nogueira et al 2008 - allometric-equations-biomass-wood-volume-amazonia]]
- [[Araújo et al 1999 - biomass-formulae-comparison-amazonia-oriental]]
- [[Melo et al 2024 - neotropical-carbon-stocks-direct-measurements-amazonia-ocidental]]

## Equações de biomassa

### Tabela 1 — Modelos de biomassa por paper

| Eq. ID | Paper        | Equação                                                                           | Variável alvo         | n    | Região           | R²    | Syx% / Erro                  |
| ------ | ------------ | --------------------------------------------------------------------------------- | --------------------- | ---- | ---------------- | ----- | ---------------------------- |
| C1     | Chave 2014   | ln(AGB) = a + b ln(ρD²H) + ε                                                      | AGB (kg)              | 4004 | Pantropical      | —     | CV 56,5% por árvore          |
| C2     | Chave 2014   | ln(AGB) = a + b ln(D²H) + ε (sem ρ)                                               | AGB (kg)              | 4004 | Pantropical      | —     | AIC = 3983 vs. 3855 (com ρ)  |
| C3     | Chave 2014   | AGBest = 0,0673 × (ρD²H)^0,976                                                    | AGB (kg)              | 4004 | Pantropical      | —     | CV 56,5% (árv.); ~10% (1 ha) |
| C4     | Chave 2014   | AGBest = exp[-1,803 − 0,976E + 0,976 ln(ρ) + 2,673 ln(D) − 0,0299(ln D)²] (Eq. 7) | AGB (kg)              | 4004 | Pantropical      | —     | CV 71,5%; bias 9,71%         |
| L1     | Lima 2012    | ln(AGW) = −2,025 + 2,459 ln D                                                     | AGW (kg)              | 101  | Rio Negro (NW)   | 0,944 | 8,40%                        |
| L2     | Lima 2012    | ln(AGW) = −3,372 + 1,830 ln D + 1,097 ln H                                        | AGW (kg)              | 101  | Rio Negro (NW)   | 0,959 | 6,58%                        |
| L3     | Lima 2012    | ln(AGW) = 5,604 + 0,957 ln(D²H)                                                   | AGW (kg)              | 101  | Rio Negro (NW)   | 0,959 | 6,59%                        |
| L4     | Lima 2012    | AGW = 0,488 × D^2,083                                                             | AGW (kg)              | 101  | Rio Negro (NW)   | 0,934 | 5,63%                        |
| L5     | Lima 2012    | AGW = 0,488 × D^2,083 × H^0,000                                                   | AGW (kg)              | 101  | Rio Negro (NW)   | 0,933 | 5,63%                        |
| L6     | Lima 2012    | AGW = 316,7 × (D²H)^0,861                                                         | AGW (kg)              | 101  | Rio Negro (NW)   | 0,920 | 6,15%                        |
| LB1    | Lima 2012    | ln(BGW) = −3,881 + 2,406 ln D                                                     | BGW (kg)              | 101  | Rio Negro (NW)   | 0,894 | 15,17%                       |
| LB2    | Lima 2012    | BGW = 0,136 × AGW                                                                 | BGW (kg)              | 101  | Rio Negro (NW)   | —     | —                            |
| S1     | Silva 2007   | PF = 2,7179 × DAP^1,8774                                                          | PF total (kg, fresco) | 494  | Manaus (Central) | 0,94  | 3,9%                         |
| S2     | Silva 2007   | PF = 0,5521 × DAP^1,6629 × HT^0,7224                                              | PF total (kg, fresco) | 494  | Manaus (Central) | 0,95  | 3,7%                         |
| SA     | Silva 2007   | AGB = 2,2737 × DAP^1,9156 × 0,584                                                 | AGB seca (kg)         | 494  | Manaus (Central) | 0,85  | 4,20%                        |
| SB     | Silva 2007   | BGB = 0,0469 × DAP^2,4754 × 0,533                                                 | BGB seca (kg)         | 131  | Manaus (Central) | 0,95  | 5,12%                        |
| H1     | Higuchi 2015 | BStot = 2,7179 × DAP^1,8774 × 0,584 × fc (fc = Hdom_sítio / 30,2)                 | BStot seca (kg)       | 494* | Amazonas         | 0,94  | 3,91%                        |
| H2     | Higuchi 2015 | AGB = 2,2737 × DAP^1,9156 × 0,584 × fc                                            | AGB seca (kg)         | 494* | Amazonas         | 0,85  | 4,20%                        |
| H3     | Higuchi 2015 | BGB = 0,0469 × DAP^2,4754 × 0,533 × fc                                            | BGB seca (kg)         | 131* | Amazonas         | 0,95  | 5,12%                        |
|        |              |                                                                                   |                       |      |                  |       |                              |

| N1 | Nogueira 2008 | ln(AGW) = −1,716 + 2,413·ln(D) | AGW seca (kg) | 267 | Sul Amazônia | — | — |
| N2 | Nogueira 2008 | AGB = 2,718·DAP^1,877·0,584·0,951 (VEF corrigido) | AGB seca (kg) | 267 | Sul Amazônia | — | — |
| A1 | Araújo 1999 | FW = 0,026·D^1,529·H^1,747 (FW7) | PF total (kg, fresca) | 127 | Pará (Leste) | — | <0,6% |
| A2 | Araújo 1999 | FW = 0,465·D^2,202/(1−M) (FW8) | PF total (kg, fresca) | 127 | Pará (Leste) | — | <0,6% |
| A3 | Araújo 1999 | ln(AGW) = −2,377 + 2,651·ln(D) (compil. Lima 2012) | AGW fresca (kg) | 127 | Pará (Leste) | — | — |

> Nota: As equações H1–H3 usam os coeficientes de Silva (2007) com fator de correção fc. n refere-se aos dados originais de Silva (2007). A equação H1 é equivalente a S1 convertida para peso seco (×0,584 = 1 − 0,416) e corrigida por fc.

### Tabela 2 — Comparação regional das equações de simples entrada (Model 1: ln DW = a + b ln D) para biomassa aérea (compilado de Lima et al., 2012, Tabela 4)

| Região                        | Fonte                  | ln AGW = a + b ln D          | R²    | Syx%  |
| ----------------------------- | ---------------------- | ---------------------------- | ----- | ----- |
| Amazônia oriental (Pará)      | Araújo et al., 1999    | ln AGW = −2,377 + 2,651 ln D | —     | —     |
| Amazônia central (Manaus)     | Silva, 2007            | ln AGW = −1,912 + 2,490 ln D | —     | —     |
| Amazônia sul (MT/PA)          | Nogueira et al., 2008a | ln AGW = −1,716 + 2,413 ln D | —     | —     |
| Amazônia noroeste (Rio Negro) | Lima et al., 2012      | ln AGW = −2,025 + 2,459 ln D | 0,944 | 8,40% |
|                               |                        |                              |       |       |

> Nota: Melo et al. (2024) fornece o primeiro conjunto de equações para uma quinta sub-região — o Sudoeste da Amazônia (SWA, Acre). Os coeficientes do modelo de simples entrada (Modelo 1: DM = a·DBH^b) devem ser consultados na publicação original (doi: 10.1016/j.foreco.2024.122195), pois o paper não os reporta no formato ln AGW = a + b·ln(D) usado na Tabela 2. A validação cruzada de Melo (2024) mostra que o Sul (Nogueira 2008) é a equação existente com menor viés no SWA (+1,3%), consistente com a similaridade fisionômica entre florestas abertas do Sul e do Sudoeste.

## Equações de altura (D-H)

### Tabela 3 — Modelos altura-diâmetro

| Eq. ID | Paper | Equação | Região | n | R² | Syx |
|--------|-------|---------|--------|----|----|-----|
| CH1 | Chave 2014 | ln(H) = 0,893 − E + 0,760 ln(D) − 0,0340[ln(D)]², onde E = (0,178×TS − 0,938×CWD − 6,61×PS)×10⁻³ | Pantropical | 4004 | — | RSE = 0,243 |
| LH7 | Lima 2012 | H = 33,42 / (1 + 1,611 × exp(−1,157 × D)) | Rio Negro (NW) | 101 | 0,846 | 1,537 m |
| LH8 | Lima 2012 | H = −6,381 + 8,785 ln D | Rio Negro (NW) | 101 | 0,846 | 1,547 m |
| LH12 | Lima 2012 | H = 37,84 / (1 + 13,34 × exp(−2,488 × D)) | Rio Negro (NW) | 101 | 0,846 | 1,537 m |

## Equações de volume

### Tabela 4 — Modelo de Berkhout (V = β0 × DAP^β1) por sítio no Amazonas (Higuchi, 2015)

| Sítio | Código | Região | n | Equação | R²aj | Incerteza |
|-------|--------|--------|---|---------|------|-----------|
| São Gabriel da Cachoeira | SGC | Alto Rio Negro | 160 | V = 0,0011 × DAP^1,9330 | 0,92 | 6,5% |
| Atalaia do Norte / Benjamin Constant | ABC | Alto Solimões | 62 | V = 0,0001 × DAP^2,5486 | 0,92 | 8,8% |
| Resex do Rio Jutaí | JUT | Triângulo Jutaí/Solimões/Juruá | 76 | V = 0,0006 × DAP^2,0640 | 0,94 | 6,7% |
| Resex do Auati-Paraná | AUP | Triângulo Jutaí/Solimões/Juruá | 127 | V = 0,0001 × DAP^2,4369 | 0,85 | 5,9% |
| Resex Lago do Capanã Grande | CAP | Região do Madeira | 177 | V = 0,0002 × DAP^2,3445 | 0,91 | 8,9% |
| Resex do Rio Unini | RUN | Alto Rio Negro | 218 | V = 0,0006 × DAP^2,1034 | 0,95 | 1,8% |
| Flona de Pau Rosa | FPR | Médio Amazonas | 219 | V = 0,0006 × DAP^2,1448 | 0,90 | 6,7% |
| Resex do Baixo Juruá | JUR | Triângulo Jutaí/Solimões/Juruá | 128 | V = 0,0007 × DAP^2,0610 | 0,94 | 5,3% |
| Rebio do Abufari | ABU | Região do Purus | 150 | V = 0,0001 × DAP^2,5761 | 0,97 | 5,3% |

## Análise por paper

### [[Chave et al 2014 - improved-allometric-models-biomass-pantropical]]

- **Objetivo**: Desenvolver modelos pan-tropicais de biomassa aérea com o maior conjunto de dados destrutivos já compilado (4004 árvores, 58 sítios, 3 continentes)
- **Modelo principal (C3)**: AGBest = 0,0673 × (ρD²H)^0,976 — modelo de potência com DAP, densidade da madeira e altura. Erro de ~56,5% por árvore, ~10% em parcelas de 1 ha
- **Inovação**: Modelo 7 (C4) substitui altura medida por variável climática composta E (deficit hídrico + sazonalidade), permitindo estimativa sem altura em campo — CV de 71,5%
- **Densidade da madeira**: Essencial — modelos sem ρ tiveram AIC 3983 vs. 3855 com ρ. Apenas 0,6% da variância residual foi explicada pelo tipo de vegetação, contra 78% pelo sítio
- **Limitação**: 6 dos 58 sítios (todos florestas úmidas) fogem do padrão geral, sugerindo que árvores com sapopemas ou medições históricas podem introduzir viés
- **Equação bioclimática (CH1)**: ln(H) = 0,893 − E + 0,760 ln(D) − 0,0340[ln(D)]², com E definido como proxy de estresse ambiental

### [[Lima et al 2012 - allometric-models-biomass-above-below-ground-rio-negro]]

- **Objetivo**: Desenvolver modelos alométricos de biomassa aérea e subterrânea para o noroeste da Amazônia (São Gabriel da Cachoeira, Rio Negro), região sem modelos específicos
- **Melhor modelo (L1)**: ln(AGW) = −2,025 + 2,459 ln D (R² = 0,944; Syx = 8,40%) — modelo de simples entrada selecionado por simplicidade, apesar de Modelos 2 e 3 terem R² maior (0,959)
- **Biomassa subterrânea (LB1)**: ln(BGW) = −3,881 + 2,406 ln D (R² = 0,894; Syx = 15,17%)
- **Razão BGW/AGW (LB2)**: BGW = 0,136 × AGW, independente do tamanho da árvore — relação consistente com a Amazônia central
- **Comparação regional (Tabela 2)**: ANCOVA mostra que a relação D-AGW difere entre Leste, Centro, Sul e Noroeste (p < 0,05), com o Noroeste apresentando as menores estimativas de biomassa para um mesmo DAP
- **Melhor modelo de altura (LH7)**: H = 33,42 / (1 + 1,611 × exp(−1,157 × D)), assíntota de 33,4 m — a menor entre as regiões amazônicas
- **Testou 6 modelos de biomassa e 6 de altura**; documentou todos os coeficientes e estatísticas

### [[Silva 2007 - allometry-stock-dynamics-biomass-manaus]]

- **Objetivo**: Desenvolver modelos alométricos atualizados para biomassa aérea, raízes grossas e total para florestas primárias e secundárias (capoeiras) em Manaus (ZF-2)
- **Modelo de simples entrada (S1)**: PF = 2,7179 × DAP^1,8774 (r² = 0,94; Syx = 3,9%) — biomassa fresca total, a mais utilizada na região
- **Modelo de dupla entrada (S2)**: PF = 0,5521 × DAP^1,6629 × HT^0,7224 (r² = 0,95; Syx = 3,7%) — pequeno ganho com inclusão da altura
- **Modelos por compartimento (SA, SB)**: AGB seca = 2,2737 × DAP^1,9156 × 0,584 (R² = 0,85); BGB seca = 0,0469 × DAP^2,4754 × 0,533 (R² = 0,95)
- **Teores**: água 41,6% (incerteza 2,8%); carbono 48,5% (incerteza 0,9%)
- **Partição**: parte aérea 72,9%; raízes grossas 27,1% da biomassa viva total
- **Custo de coleta**: R$ 805 ± 310 por árvore (biomassa total); 100 árvores suficientes para erro < 10%

### [[Higuchi 2015 - volume-biomass-carbon-dynamics-amazonas]]

- **Objetivo**: Estimar estoques de volume e carbono para o estado do Amazonas usando 1128 parcelas em 11 localidades
- **Equações de volume (Tabela 4)**: Ajustou o modelo de Berkhout (V = β0 × DAP^β1) para 9 sítios, com n variando de 62 (ABC) a 219 (FPR) árvores cubadas. R²aj de 0,85 (AUP) a 0,97 (ABU); incerteza de 1,8% (RUN) a 8,9% (CAP)
- **Equação de biomassa (H1–H3)**: Adotou as equações de Silva (2007) corrigidas por fator fc = Hdom_sítio / Hdom_Manaus (30,2 m). Aplica conversão para peso seco (×0,584) e para carbono (×0,485)
- **ANCOVA**: Rejeitou equação de volume única para todo o estado (p < 0,000001), corroborando a necessidade de equações específicas por sítio
- **Sítios sem equação própria (MIL, ZF5)**: Utilizaram equações de sítios vizinhos ou dados históricos

### [[Nogueira et al 2008 - allometric-equations-biomass-wood-volume-amazonia]]

- **Objetivo**: Desenvolver equações alométricas de biomassa e volume para florestas abertas do sul da Amazônia (SA), ajustar fatores de conversão de volume (VEF, BEF) e produzir novo mapa de biomassa para a Amazônia Legal Brasileira
- **Modelo de simples entrada (N1)**: ln(AGW) = −1,716 + 2,413·ln(D) — calibrado com 267 árvores (5–124 cm DAP) em MT, PA e RO
- **Validação cruzada**: Equações da Amazônia Central superestimam biomassa na SA em 6–19% — a maior diferença ocorre nas classes de DAP inferiores (<30 cm), evidenciando que a alocação diferencial de biomassa entre fuste e copa é o principal fator
- **Proporção de copa**: 39,4% da biomassa total na SA vs. valores menores na CA — fustes mais curtos e copas mais pesadas explicam o viés
- **Fator de forma**: 0,7 do RadamBrasil é adequado para árvores ≥31,8 cm DAP; para classes menores, VEF precisa de correção de ~25%
- **BEF**: O fator de expansão de biomassa de copa superestima em 6% na floresta densa e ~18% na floresta aberta — erro sistemático que se propaga para estimativas de carbono
- **Mapa final**: 123,1 Gt peso seco (1976); 105,4 Gt (2006, após 676.000 km² desmatados) — ~51,1 Gt C

### [[Araújo et al 1999 - biomass-formulae-comparison-amazonia-oriental]]

- **Objetivo**: Testar 14 equações alométricas da literatura contra dados reais de pesagem destrutiva de 127 árvores em Tomé-Açu (PA) para identificar as mais acuradas para a Amazônia oriental
- **Melhor modelo (A1 — FW7)**: FW = 0,026·D^1,529·H^1,747 — erro <0,6% do peso real em campo. Combina DAP e altura como preditores
- **Melhor modelo sem altura (A2 — FW8)**: FW = 0,465·D^2,202/(1−M) — erro <0,6%. Usa umidade da madeira (M) como segundo preditor; vantagem quando a altura não está disponível
- **Equações de Higuchi & Carvalho (1994)**: Tiveram desempenho razoável fora de sua região de calibração (Manaus → Pará), mas erros aumentaram nas classes extremas de DAP
- **Equações de Overman et al. (1994)**: Da Colômbia, tiveram os maiores erros, confirmando que equações de outras regiões biogeográficas têm baixa transferibilidade para a Amazônia oriental
- **Limitação**: Apenas 0,2 ha amostrados (127 árvores) — uma única árvore grande (Ceiba pentandra) distorceu a extrapolação direta para 1 ha (848 t ha⁻¹ por pesagem direta vs. 275–597 t ha⁻¹ por equações)

### [[Melo et al 2024 - neotropical-carbon-stocks-direct-measurements-amazonia-ocidental]]

- **Objetivo**: Calibrar o primeiro conjunto de equações alométricas e teores de carbono especificamente para o Sudoeste da Amazônia (SWA — Acre), região sem dados destrutivos prévios, e validar equações existentes
- **Amostragem**: 190 árvores (5–90 cm DAP) em 20 parcelas de 100 m² na Floresta Estadual do Antimary (ASF), divididas entre floresta aberta com bambu (Guadua weberbaueri) e sem bambu
- **Modelos recomendados**: Modelo 1 (DM = a·DBH^b, MQO) e Modelo 4 (ln(DM) = ln(a) + b·ln(DBH), MQN) — os mais práticos para o SWA. Os coeficientes específicos devem ser consultados na publicação original
- **Validação cruzada (contribuição central)**: Quantificou o viés de cada equação regional quando aplicada ao SWA — Leste superestima 37,1% (±1,5); Centro superestima 13,3% (±2,1); Sul superestima 1,3% (±3,1); Noroeste subestima 1,3% (±3,1). A similaridade entre Sul e SWA (ambos florestas abertas) é consistente com o menor viés observado
- **Chave (2014)**: Equação 4 superestima 26% (±16%); Equação 7 superestima 46% (±17%) no SWA — o maior viés documentado para um modelo pantropical em uma sub-região amazônica
- **Teor de carbono**: 44,3% (±0,3) AGB e 44,6% (±0,2) BGB — ~4% menor que o valor de Silva (2007) para Manaus (48,5%), com implicações diretas para estimativas de carbono em projetos REDD+ no SWA
- **Razão BGB:AGB**: 0,167 (±0,017), superior aos 0,136 encontrados no Centro e Noroeste. O fator IPCC (0,37) superestima biomassa subterrânea em 20% no SWA

## Conclusões da síntese

1. **A escolha entre modelos de simples e dupla entrada tem impacto modesto na precisão.** Em todos os estudos regionais, incluir altura melhora R² em ~0,01–0,02 pontos e reduz Syx em ~0,2–1,8 pontos percentuais, mas o ganho é pequeno frente ao custo de medir altura em campo (Lima, 2012; Silva, 2007).

2. **Modelos pan-tropicais vs. regionais é o principal ponto de divergência.** Chave (2014) demonstra que um modelo único (C3) atinge ~10% de erro por hectare globalmente, mas Lima (2012) e Higuchi (2015) mostram que diferenças regionais na relação D-H (assíntota de 33,4 m no NW vs. 41,4 m no Centro) produzem viés sistemático quando um modelo geral é aplicado localmente (Chave, 2014: 78% da variância residual explicada pelo sítio).

3. **A densidade da madeira é o preditor mais subutilizado.** Apenas Chave (2014) a incorpora, demonstrando redução significativa de erro. Nenhum dos modelos regionais amazônicos (Silva, 2007; Lima, 2012; Higuchi, 2015) inclui ρ, o que representa uma limitação documentada.

4. **O modelo de Berkhout (V = β0 × DAP^β1) foi o mais adequado para volume na Amazônia** entre 5 modelos testados por Higuchi (2015). Os coeficientes variam substancialmente entre sítios (β0 de 0,0001 a 0,0011; β1 de 1,93 a 2,58), reforçando a necessidade de calibração local.

5. **A razão BGW/AGW é consistente entre regiões.** Lima (2012) encontrou 0,136 para o noroeste, valor similar ao documentado por Silva (2007) para a Amazônia central, sugerindo que esta relação pode ser invariante entre formações de terra firme.

6. **Os níveis de incerteza não são diretamente comparáveis entre os estudos** devido ao uso de métricas diferentes: Chave (2014) reporta CV%; Lima (2012) reporta Syx% e R²; Silva (2007) reporta r² e Syx%; Higuchi (2015) reporta R²aj e IC 95% amostral. A falta de padronização dificulta a hierarquização da precisão entre modelos.

7. **O viés regional é o maior fator de incerteza em estimativas de biomassa amazônica.** Aplicar equações de uma sub-região em outra produz erros de 6–19% (Nogueira, 2008: CA→SA), 13–37% (Melo, 2024: Leste/Centro→SWA), ou completamente invalida a estimativa (Araújo, 1999: Overman/Colômbia→Pará). A validação cruzada entre as cinco sub-regiões hoje documentadas (Leste, Centro, Sul, Noroeste, Sudoeste) mostra que o erro sistemático supera o erro aleatório dos modelos.

8. **Fatores de expansão (VEF, BEF) requerem calibração regional tanto quanto as equações alométricas.** Nogueira (2008) mostra que VEF para árvores 10–31,7 cm DAP estava subestimado em ~25% e BEF superestima em 6–18% dependendo do tipo florestal — erros que se propagam para estimativas de carbono em escala regional.

9. **O modelo ln(AGW) = a + b·ln(D) (simples entrada) é o formato mais replicável entre regiões**, permitindo comparação direta de coeficientes (Tabela 2). As inclinações (b) variam de 2,413 (Sul) a 2,651 (Leste), e os interceptos (a) de −2,377 (Leste) a −1,716 (Sul), indicando que a estrutura alométrica difere sistematicamente entre sub-regiões.

## Perguntas em aberto

- Qual o ganho real de precisão ao incluir densidade da madeira (ρ) nos modelos regionais da Amazônia, dado que sua medição requer laboratório e aumenta o custo de coleta?
- O fator de correção por Hdom (Higuchi, 2015) pode ser validado com dados independentes de outros estados amazônicos (Pará, Mato Grosso, Acre)?
- A razão BGW/AGW de ~0,136 se mantém em florestas de várzea, igapó e campinas, ou é exclusiva de terra firme?
- O modelo FW8 de Araújo (1999), que usa umidade da madeira (M) em vez de altura, pode ser calibrado para outras regiões como alternativa de baixo custo operacional?
- Qual o erro de se aplicar a equação de simples entrada do Sul (Nogueira 2008: b = 2,413) nas florestas abertas do Sudoeste (Melo 2024), dado que são fisionomicamente similares?

## Recomendação por região

Com base na validação cruzada disponível, a recomendação abaixo prioriza equações **calibradas e validadas na própria região**. Quando não há equação específica, sugere-se a melhor alternativa com o viés esperado.

| Região | Equação recomendada | Base | Aplicabilidade | Viés esperado se usar outra |
|--------|-------------------|------|----------------|------------------------------|
| **Amazônia Central** (Manaus, ZF-2) | Silva (2007) — **S2**: PF = 0,5521·DAP^1,6629·HT^0,7224 (r² = 0,95; Syx = 3,7%) | 494 árvores, Manaus | Floresta densa de terra firme. Usar S1 se altura não disponível: PF = 2,7179·DAP^1,8774 (r² = 0,94; Syx = 3,9%) | Equações do Leste superestimam; Sul subestima 6–19% |
| **Amazônia Oriental** (Pará, Tomé-Açu) | Araújo (1999) — **A1 (FW7)**: FW = 0,026·D^1,529·H^1,747 (erro <0,6%) | 127 árvores, Tomé-Açu | Floresta de terra firme do leste. **A2 (FW8)** se altura incerta: FW = 0,465·D^2,202/(1−M) | Equações do Centro superestimam; Colômbia (Overman) inviável |
| **Amazônia Meridional** (MT, PA, RO — florestas abertas) | Nogueira (2008) — **N1**: ln(AGW) = −1,716 + 2,413·ln(D) | 267 árvores, sul da Amazônia | Floresta aberta com copas mais pesadas e fustes mais curtos. Não usar equações de floresta densa sem correção | Amazônia Central superestima 6–19%; Leste superestima mais |
| **Noroeste (Alto Rio Negro)** | Lima (2012) — **L1**: ln(AGW) = −2,025 + 2,459·ln(D) (R² = 0,944; Syx = 8,40%) | 101 árvores, SGC | Floresta densa de terra firme com as menores assíntotas de altura. **L4**: AGW = 0,488·D^2,083 para uso sem log | Chave (2014) superestima (assíntota H maior); Centro também superestima |
| **Sudoeste (Acre, SWA)** | Melo (2024) — Modelo 1: DM = a·DBH^b (ver nota original para coeficientes) | 190 árvores, Antimary | Floresta aberta com bambu e sem bambu. Teor de C ~44,3% (menor que o padrão) | Chave (2014) superestima 26–46%; Leste superestima 37%; Centro superestima 13% |
| **Estado do Amazonas (volume)** | Higuchi (2015) — Berkhout V = β0·DAP^β1 por sítio (Tabela 4) | 62–219 árvores por sítio | Equação de volume específica por sítio (9 sítios). Usar fc = Hdom_sítio / 30,2 se aplicar equações de biomassa de Silva (2007) | Equação única para todo o AM rejeitada por ANCOVA (p < 0,000001) |
| **Toda a Amazônia (sem dados locais)** | Chave (2014) — **C3**: AGBest = 0,0673 × (ρD²H)^0,976 | 4004 árvores, 58 sítios | Cenário sem equação regional. Incluir ρ reduz erro substancialmente. Erro ~10% por hectare, mas viés sistemático de até 46% em sub-regiões | Preferir equação regional sempre que disponível |

Notas importantes:

1. **Hierarquia de escolha**: (a) equação calibrada na mesma região e tipo florestal → (b) equação de região fisionomicamente similar → (c) modelo pantropical com ρ medido → (d) modelo pantropical sem ρ
2. **Conversão fresco→seco**: Aplicar teor de umidade regional. Valores disponíveis: Manaus 41,6% (Silva, 2007), SWA 47,0% (Melo, 2024), Sul 41,6% fuste / 47,6% copa (Nogueira, 2008), Leste ~40% (Araújo, 1999)
3. **Conversão seco→carbono**: Teor de C varia de 44,3% (SWA, Melo 2024) a 48,5% (Manaus, Silva 2007). Usar 0,485 como default, mas calibrar se houver dados regionais
4. **Razão BGB:AGB**: Usar 0,136 (Lima, 2012; Silva, 2007) para terra firme, com cautela. Melo (2024) encontrou 0,167 para SWA — IPCC recomenda 0,37, que superestima em 20% no SWA
5. **Sítios sem equação própria dentro do Amazonas**: Higuchi (2015) fornece fc = Hdom_sítio / 30,2 como alternativa para usar equações de Silva (2007) corrigidas por altura dominante do sítio
