# sprint9 - Projeto de Priorização de Hipóteses e Análise de Teste A/B

Este projeto foca na otimização de receita de uma loja online através de uma abordagem orientada a dados, dividida em duas frentes: a priorização estratégica de hipóteses de negócio e a análise rigorosa de um Teste A/B para validação de resultados.

## Contexto do Problema
O objetivo era identificar quais mudanças no produto trariam o maior retorno sobre o investimento (ROI) e validar, através de um experimento controlado, se uma nova implementação de fato alteraria as métricas de conversão e receita da plataforma.

## Stack Tecnológica
Linguagem: Python
Bibliotecas: Pandas, NumPy (Processamento), Matplotlib/Seaborn (Visualização), Scipy (Estatística)
Metodologias: Frameworks RICE e ICE, Testes de Significância Estatística (Z-test), Análise de Séries Temporais.

## Etapas do Projeto
1. Priorização de Hipóteses (Framework RICE)
Em vez de testar ideias aleatoriamente, utilizei o framework RICE (Reach, Impact, Confidence, Effort) para ranquear 9 hipóteses de negócio.
Destaque Técnico: A transição do ICE para o RICE alterou drasticamente o ranking, evidenciando como o fator Alcance (Reach) é crucial para decisões que impactam a receita em escala.

2. Análise de Teste A/B e Estabilidade de Métricas
Análise do comportamento dos Grupos A e B através de:
- Receita acumulada e tamanho médio do pedido acumulado.
- Taxas de conversão diárias.
- Cálculo de anomalias e outliers (usuários com número excessivo de pedidos ou valores fora da curva) para limpar o ruído estatístico.

3. Testes de Hipóteses Estatísticas
Apliquei o teste de Wilcoxon-Mann-Whitney para dados não paramétricos e analisei a significância estatística das diferenças na conversão e no ticket médio.
