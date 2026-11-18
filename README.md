# 🇧🇷 Imposto das Brusinhas
### Análise de Dados das Importações Brasileiras de Vestuário (2023–2026)

## 📌 Sobre o projeto

Este projeto tem como objetivo analisar o comportamento das importações brasileiras de vestuário entre 2023 e 2026, investigando a evolução dos valores importados e as mudanças na participação dos países de origem.

O estudo tem como foco a alteração na tributação das compras internacionais de até US$ 50 realizadas por meio do Programa Remessa Conforme, com redução da alíquota do Imposto de Importação para 0% a partir de 12 de maio de 2026.

A proposta é utilizar dados públicos para identificar movimentos no comércio exterior brasileiro e transformar grandes volumes de dados em informações relevantes para análise e tomada de decisão.

## 🎯 Objetivos

- Analisar a evolução mensal do valor FOB das importações brasileiras de vestuário.
- Comparar o comportamento das importações antes e depois da mudança tributária de maio de 2026.
- Identificar países que ganharam participação no valor FOB das importações.
- Avaliar mudanças na distribuição dos países de origem.

## 📊 Fonte de dados

**Comex Stat — Ministério do Desenvolvimento, Indústria, Comércio e Serviços (MDIC)**

Os dados utilizados são provenientes das bases públicas de comércio exterior brasileiro.

- Período: 2023 a 2026.
- Produtos: capítulos 61 e 62 da NCM (vestuário).
- Indicador principal: valor FOB, em dólares americanos (US$).
- Período disponível de 2026: janeiro a outubro.

Fonte: https://comexstat.mdic.gov.br/

## 🛠️ Ferramentas e tecnologias

- **Python:** tratamento e preparação dos dados.
- **Pandas:** manipulação e análise de dados.
- **Jupyter Notebook:** exploração e desenvolvimento das análises.
- **Power BI:** construção do dashboard e visualização dos resultados.
- **SQL / PL-SQL:** conhecimentos aplicados à lógica de consulta e análise de dados.

## 🔎 Metodologia

O projeto foi desenvolvido em etapas:

1. Obtenção dos dados públicos de importação.
2. Filtragem das operações relacionadas aos capítulos 61 e 62 da NCM.
3. Tratamento e consolidação das bases anuais.
4. Análise da evolução mensal do valor FOB.
5. Comparação dos períodos de janeiro a abril e junho a setembro de 2026.
6. Cálculo da participação percentual dos países e de sua variação em pontos percentuais.
7. Construção de dashboard no Power BI.

Maio de 2026 foi excluído da comparação principal por ser o mês de implementação da mudança tributária, ocorrida em 12/05/2026.

## 📈 Principais resultados

Na comparação entre janeiro–abril e junho–setembro de 2026:

- O valor FOB passou de aproximadamente US$ 1,108 bilhão para US$ 906 milhões, uma redução de 18,25%.
- A participação da China passou de 60,53% para 50,07%, uma redução de 10,46 pontos percentuais.
- Entre os países com maiores ganhos de participação estão Vietnã, Peru, Paraguai, Camboja e Turquia.

## ⚠️ Limitações da análise

Os dados do Comex Stat representam importações agregadas e não identificam:

- Plataformas de comércio eletrônico específicas, como Shein, Shopee, AliExpress ou Temu.
- Compras individuais ou encomendas de consumidores.
- Valor individual de cada encomenda.
- Elegibilidade de cada operação às regras do Programa Remessa Conforme.

Portanto, os resultados demonstram movimentos observados após a mudança tributária, mas não permitem afirmar que a redução do imposto foi a causa direta das variações identificadas.

## 📁 Estrutura do projeto

```text
imposto-das-brusinhas/
│
├── dados/
├── notebooks/
├── powerbi/
├── imagens/
├── README.md
└── requirements.txt
```

## 🚀 Objetivo de aprendizado

Este projeto também faz parte da minha jornada de desenvolvimento em Análise de Dados e Business Intelligence, aplicando conhecimentos de programação, tratamento de dados, análise exploratória e visualização de informações a um problema real.

---

**Projeto desenvolvido para fins de estudo e portfólio em Análise de Dados.**
