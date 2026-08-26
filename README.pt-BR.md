# Air Quality Data Analysis

Análise exploratória de dados de qualidade do ar coletados em uma área urbana de **Milão, Itália**, entre março de 2004 e fevereiro de 2005.

O projeto investiga como fatores climáticos e temporais estão associados às concentrações de poluentes atmosféricos, utilizando **Python e técnicas de análise exploratória de dados**.

---

## Objetivo

Analisar os níveis de poluição atmosférica e identificar padrões e possíveis relações entre:

- `CO(GT)` — Monóxido de carbono
- `NOx(GT)` — Óxidos de nitrogênio
- `NO2(GT)` — Dióxido de nitrogênio
- Temperatura
- Umidade
- Horário do dia
- Sensores químicos `PT08`

---

## Hipóteses investigadas

A análise foi estruturada a partir de seis hipóteses:

**H1 — Temperatura e poluição**  
Temperaturas mais baixas estão associadas a maiores concentrações de poluentes?

**H2 — Umidade e poluição**  
Níveis mais elevados de umidade estão associados a maiores concentrações de gases poluentes?

**H3 — Períodos frios e óxidos de nitrogênio**  
Períodos de menor temperatura apresentam maiores concentrações de NOx e NO₂?

**H4 — Padrões ao longo do dia**  
As concentrações de CO, NOx e NO₂ variam de acordo com o horário?

**H5 — Relação entre NOx e NO₂**  
Os dois poluentes apresentam comportamento temporal semelhante?

**H6 — Sensores PT08**  
As respostas dos sensores apresentam comportamento semelhante às medições de referência?

---

##  Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Google Colab
- Jupyter Notebook

---

##  Metodologia

O projeto foi desenvolvido seguindo as principais etapas de uma análise exploratória de dados:

1. Entendimento do conjunto de dados
2. Inspeção inicial
3. Limpeza e tratamento dos dados
4. Estatísticas descritivas
5. Análise univariada
6. Análise bivariada e multivariada
7. Investigação das hipóteses
8. Identificação de padrões
9. Comunicação dos resultados

Durante a preparação dos dados, valores `-200`, utilizados para representar medições ausentes ou inválidas, foram tratados como valores ausentes (`NaN`). As informações de data e hora também foram combinadas em uma variável `Datetime`, permitindo análises temporais.

---

##  Principais resultados

A análise revelou uma associação importante entre **temperatura e óxidos de nitrogênio**. O NOx apresentou concentrações progressivamente maiores nas menores faixas de temperatura, enquanto o NO₂ também apresentou valores médios superiores nos períodos mais frios.

A comparação direta entre períodos frios e mais quentes reforçou esse resultado: **NOx e NO₂ apresentaram maiores concentrações médias nos períodos classificados como frios**.

Também foram identificados padrões ao longo das 24 horas. CO, NOx e NO₂ apresentaram variações de concentração de acordo com o horário, com elevações durante a manhã e, principalmente, no final da tarde e início da noite.

A relação com a umidade mostrou-se diferente para cada poluente. O NOx apresentou aumento nas maiores faixas de umidade relativa, enquanto CO apresentou pequenas variações e NO₂ comportamento distinto.

NOx e NO₂ também apresentaram tendências temporais semelhantes em determinados períodos, embora diferenças na intensidade e no momento dos picos indiquem que seus comportamentos não são completamente equivalentes.

Por fim, as respostas dos sensores PT08 analisados não acompanharam de maneira consistente as respectivas medições de referência, abrindo possibilidades para estudos futuros relacionados à calibração e ao desempenho desses sensores.

> Os resultados representam associações observadas no conjunto de dados e não devem ser interpretados como evidência de causalidade.

---

##  Conclusão

Os resultados mostram que fatores **climáticos e temporais estão associados de maneiras distintas ao comportamento da poluição atmosférica**.

Entre os padrões encontrados, destacam-se a maior concentração de NOx e NO₂ em períodos frios e as variações dos níveis de poluição ao longo das diferentes horas do dia.

O projeto também evidencia como a análise exploratória de dados pode transformar medições ambientais em informações capazes de revelar padrões e gerar novas hipóteses de investigação.

---

## Próximos passos

Como continuidade do projeto, podem ser explorados:

- modelos de Machine Learning para previsão de níveis de poluição;
- análise mais aprofundada da sazonalidade;
- identificação automática de episódios atípicos de poluição;
- avaliação e calibração dos sensores PT08;
- construção de dashboards interativos para monitoramento da qualidade do ar.

---

## Autora

**Annanda Bispo**  
Engenharia da Computação — UFRN

Projeto desenvolvido para estudo e portfólio em **Análise de Dados, Ciência de Dados e Inteligência Artificial**.
