---
noteId: "sintese-equacoes-alometricas"
tags:
  - "biomassa"
  - "amazonia"
  - "metodologia"
---

# Síntese - Equações alométricas para biomassa e volume na Amazônia

## Resumo em uma frase

Os quatro papers fornecem 23 equações alométricas documentadas (15 para biomassa, 9 para volume, 3 para altura), abrangendo desde modelos pan-tropicais com 4004 árvores (Chave et al., 2014) até equações de volume específicas por sítio com 62–219 árvores cada (Higuchi, 2015), com R² variando de 0,85 a 0,97 e erro padrão de 1,8% a 15,17%.

## Papers consultados

- [[Chave et al 2014 - improved-allometric-models-biomass-pantropical]]
- [[Lima et al 2012 - allometric-models-biomass-above-below-ground-rio-negro]]
- [[Silva 2007 - allometry-stock-dynamics-biomass-manaus]]
- [[Higuchi 2015 - volume-biomass-carbon-dynamics-amazonas]]

## Equações de biomassa

### Tabela 1 — Modelos de biomassa por paper

| Eq. ID | Paper | Equação | Variável alvo | n | Região | R² | Syx% / Erro |
|--------|-------|---------|---------------|----|--------|----|-------------|
| C1 | Chave 2014 | ln(AGB) = a + b ln(ρD²H) + ε | AGB (kg) | 4004 | Pantropical | — | CV 56,5% por árvore |
| C2 | Chave 2014 | ln(AGB) = a + b ln(D²H) + ε (sem ρ) | AGB (kg) | 4004 | Pantropical | — | AIC = 3983 vs. 3855 (com ρ) |
| C3 | Chave 2014 | AGBest = 0,0673 × (ρD²H)^0,976 | AGB (kg) | 4004 | Pantropical | — | CV 56,5% (árv.); ~10% (1 ha) |
| C4 | Chave 2014 | AGBest = exp[-1,803 − 0,976E + 0,976 ln(ρ) + 2,673 ln(D) − 0,0299(ln D)²] (Eq. 7) | AGB (kg) | 4004 | Pantropical | — | CV 71,5%; bias 9,71% |
| L1 | Lima 2012 | ln(AGW) = −2,025 + 2,459 ln D | AGW (kg) | 101 | Rio Negro (NW) | 0,944 | 8,40% |
| L2 | Lima 2012 | ln(AGW) = −3,372 + 1,830 ln D + 1,097 ln H | AGW (kg) | 101 | Rio Negro (NW) | 0,959 | 6,58% |
| L3 | Lima 2012 | ln(AGW) = 5,604 + 0,957 ln(D²H) | AGW (kg) | 101 | Rio Negro (NW) | 0,959 | 6,59% |
| L4 | Lima 2012 | AGW = 0,488 × D^2,083 | AGW (kg) | 101 | Rio Negro (NW) | 0,934 | 5,63% |
| L5 | Lima 2012 | AGW = 0,488 × D^2,083 × H^0,000 | AGW (kg) | 101 | Rio Negro (NW) | 0,933 | 5,63% |
| L6 | Lima 2012 | AGW = 316,7 × (D²H)^0,861 | AGW (kg) | 101 | Rio Negro (NW) | 0,920 | 6,15% |
| LB1 | Lima 2012 | ln(BGW) = −3,881 + 2,406 ln D | BGW (kg) | 101 | Rio Negro (NW) | 0,894 | 15,17% |
| LB2 | Lima 2012 | BGW = 0,136 × AGW | BGW (kg) | 101 | Rio Negro (NW) | — | — |
| S1 | Silva 2007 | PF = 2,7179 × DAP^1,8774 | PF total (kg, fresco) | 494 | Manaus (Central) | 0,94 | 3,9% |
| S2 | Silva 2007 | PF = 0,5521 × DAP^1,6629 × HT^0,7224 | PF total (kg, fresco) | 494 | Manaus (Central) | 0,95 | 3,7% |
| SA | Silva 2007 | AGB = 2,2737 × DAP^1,9156 × 0,584 | AGB seca (kg) | 494 | Manaus (Central) | 0,85 | 4,20% |
| SB | Silva 2007 | BGB = 0,0469 × DAP^2,4754 × 0,533 | BGB seca (kg) | 131 | Manaus (Central) | 0,95 | 5,12% |
| H1 | Higuchi 2015 | BStot = 2,7179 × DAP^1,8774 × 0,584 × fc (fc = Hdom_sítio / 30,2) | BStot seca (kg) | 494* | Amazonas | 0,94 | 3,91% |
| H2 | Higuchi 2015 | AGB = 2,2737 × DAP^1,9156 × 0,584 × fc | AGB seca (kg) | 494* | Amazonas | 0,85 | 4,20% |
| H3 | Higuchi 2015 | BGB = 0,0469 × DAP^2,4754 × 0,533 × fc | BGB seca (kg) | 131* | Amazonas | 0,95 | 5,12% |

*Nota: As equações H1–H3 usam os coeficientes de Silva (2007) com fator de correção fc. n refere-se aos dados originais de Silva (2007). A equação H1 é equivalente a S1 convertida para peso seco (×0,584 = 1 − 0,416) e corrigida por fc.

### Tabela 2 — Comparação regional das equações de simples entrada (Model 1: ln DW = a + b ln D) para biomassa aérea (compilado de Lima et al., 2012, Tabela 4)

| Região | Fonte | ln AGW = a + b ln D | R² | Syx% |
|--------|-------|-------------------|----|------|
| Amazônia oriental (Pará) | Araújo et al., 1999 | ln AGW = −2,377 + 2,651 ln D | — | — |
| Amazônia central (Manaus) | Silva, 2007 | ln AGW = −1,912 + 2,490 ln D | — | — |
| Amazônia sul (MT/PA) | Nogueira et al., 2008a | ln AGW = −1,716 + 2,413 ln D | — | — |
| Amazônia noroeste (Rio Negro) | Lima et al., 2012 | ln AGW = −2,025 + 2,459 ln D | 0,944 | 8,40% |

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

## Conclusões da síntese

1. **A escolha entre modelos de simples e dupla entrada tem impacto modesto na precisão.** Em todos os estudos regionais, incluir altura melhora R² em ~0,01–0,02 pontos e reduz Syx em ~0,2–1,8 pontos percentuais, mas o ganho é pequeno frente ao custo de medir altura em campo (Lima, 2012; Silva, 2007).

2. **Modelos pan-tropicais vs. regionais é o principal ponto de divergência.** Chave (2014) demonstra que um modelo único (C3) atinge ~10% de erro por hectare globalmente, mas Lima (2012) e Higuchi (2015) mostram que diferenças regionais na relação D-H (assíntota de 33,4 m no NW vs. 41,4 m no Centro) produzem viés sistemático quando um modelo geral é aplicado localmente (Chave, 2014: 78% da variância residual explicada pelo sítio).

3. **A densidade da madeira é o preditor mais subutilizado.** Apenas Chave (2014) a incorpora, demonstrando redução significativa de erro. Nenhum dos modelos regionais amazônicos (Silva, 2007; Lima, 2012; Higuchi, 2015) inclui ρ, o que representa uma limitação documentada.

4. **O modelo de Berkhout (V = β0 × DAP^β1) foi o mais adequado para volume na Amazônia** entre 5 modelos testados por Higuchi (2015). Os coeficientes variam substancialmente entre sítios (β0 de 0,0001 a 0,0011; β1 de 1,93 a 2,58), reforçando a necessidade de calibração local.

5. **A razão BGW/AGW é consistente entre regiões.** Lima (2012) encontrou 0,136 para o noroeste, valor similar ao documentado por Silva (2007) para a Amazônia central, sugerindo que esta relação pode ser invariante entre formações de terra firme.

6. **Os níveis de incerteza não são diretamente comparáveis entre os estudos** devido ao uso de métricas diferentes: Chave (2014) reporta CV%; Lima (2012) reporta Syx% e R²; Silva (2007) reporta r² e Syx%; Higuchi (2015) reporta R²aj e IC 95% amostral. A falta de padronização dificulta a hierarquização da precisão entre modelos.

## Perguntas em aberto

- Qual o ganho real de precisão ao incluir densidade da madeira (ρ) nos modelos regionais da Amazônia, dado que sua medição requer laboratório e aumenta o custo de coleta?
- O fator de correção por Hdom (Higuchi, 2015) pode ser validado com dados independentes de outros estados amazônicos (Pará, Mato Grosso, Acre)?
- A razão BGW/AGW de ~0,136 se mantém em florestas de várzea, igapó e campinas, ou é exclusiva de terra firme?
