# imposto-das-brusinhas

Análise das importações brasileiras de vestuário (2023–2026) e do que mudou depois do fim do imposto de importação sobre compras internacionais de até US$ 50.

> Projeto de estudo e portfólio em Análise de Dados.

## contexto

Desde 12/05/2026, compras internacionais de até US$ 50 feitas pelo Programa Remessa Conforme passaram a ter alíquota de Imposto de Importação de 0%.

A pergunta do projeto: **o que aparece nos dados públicos de comércio exterior depois dessa mudança?**

## perguntas

- Como evoluiu o valor FOB mensal das importações de vestuário?
- O comportamento muda antes e depois de maio de 2026?
- Quais países ganharam participação?
- A distribuição dos países de origem mudou?

## dados

| item | detalhe |
|---|---|
| fonte | [Comex Stat (MDIC)](https://comexstat.mdic.gov.br/) |
| período | 2023 a 2026 (2026: jan–out) |
| produtos | NCM capítulos 61 e 62 (vestuário) |
| métrica | valor FOB em US$ |

## stack

```
python · pandas · jupyter notebook · power bi
```

SQL / PL-SQL entram na lógica de consulta e agregação.

## como foi feito

1. Download das bases públicas de importação
2. Filtro nos capítulos 61 e 62 da NCM
3. Tratamento e consolidação das bases anuais
4. Análise da evolução mensal do valor FOB
5. Comparação de **jan–abr** vs **jun–set** de 2026
6. Cálculo da participação (%) por país e variação em pontos percentuais
7. Dashboard no Power BI

Maio/2026 ficou **fora** da comparação principal, por ser o mês em que a mudança entrou em vigor (12/05).

## resultados

Comparando jan–abr com jun–set de 2026:

| indicador | antes | depois | variação |
|---|---|---|---|
| valor FOB | ~US$ 1,108 bi | US$ 906 mi | -18,25% |
| participação da China | 60,53% | 50,07% | -10,46 p.p. |

Maiores ganhos de participação: Vietnã, Peru, Paraguai, Camboja e Turquia.

## limitações

Os dados do Comex Stat são agregados. Eles **não** identificam:

- plataformas específicas (Shein, Shopee, AliExpress, Temu)
- compras individuais de consumidores
- o valor de cada encomenda
- se cada operação se enquadra no Remessa Conforme

Os resultados mostram movimentos observados depois da mudança tributária. Eles **não** permitem afirmar que a redução do imposto causou essas variações.

## estrutura

```text
imposto-das-brusinhas/
├── dados/
├── notebooks/
├── powerbi/
├── imagens/
├── README.md
└── requirements.txt
```

## rodando localmente

```bash
git clone https://github.com/<seu-usuario>/imposto-das-brusinhas.git
cd imposto-das-brusinhas
pip install -r requirements.txt
jupyter notebook notebooks/
```

## sobre

Parte da minha transição para Análise de Dados e BI: programação, tratamento de dados, análise exploratória e visualização aplicadas a um problema real.

**Débora Costa** · [LinkedIn](https://www.linkedin.com/in/deboracosttaa)
