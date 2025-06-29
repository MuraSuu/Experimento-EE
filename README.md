# Análise Exploratória do SAEB 2023 – Ensino Médio

Se trata de um projeto para aplicar o que eu aprendi nos ultimos 4 meses em relação a tecnicas de estatistica exploratoria. Algumas coisas vem de aulas, livros ou até mesmo blogs.

## Objetivo

O notebook tem duas partes. 

A primeira se trata de uma analise bivariada entre as notas de proeficiencia em matematica e portugues.

Explorar a relação entre o histórico de reprovação dos estudantes e suas respostas às seguintes questões do questionário do SAEB:

- **TX_RESP_Q19**: “Você já foi reprovado?”
- **TX_RESP_Q23a**: “Me interesso pelo que foi ensinado esse ano”
- **TX_RESP_Q23b**: “Me sinto motivado a usar o que foi ensinado esse ano”

Inicialmente, a hipótese era de que estudantes reprovados apresentariam menor interesse ou motivação.

## Fontes

- Dados: [INEP - SAEB 2023](https://www.gov.br/inep/pt-br/areas-de-atuacao/avaliacao-e-exames-educacionais/saeb)
- Documentação: Dicionário de variáveis e estrutura dos microdados disponíveis no portal do INEP.

## Tecnologias e bibliotecas

- Python 3.x
- pandas
- seaborn
- matplotlib
- scipy
- JupyterLab

## O que foi feito

- Limpeza e filtragem das respostas qualitativas (substituição de valores não respondidos).
- Mapeamento das letras para categorias ordenadas (Likert).
- Tabelas de contingência para cruzamento de respostas.
- Testes de independência usando qui-quadrado.
- Teste de associção usando spearman.
- Visualizações com heatmaps e interpretação descritiva.

## Principais conclusões

- Não há associação estatisticamente significativa entre histórico de reprovação e as respostas de interesse ou motivação dos estudantes (valor-p ≈ 0.99).
- Os coeficientes de associação (como Cramer's V) também indicam dependência fraca entre as variáveis.
- As notas de matematica e portugues tem uma relação positiva, porem não linear por conta de algum tipo de heteroscedasticidade.

## Como rodar

Basta abrir o notebook `.ipynb` com JupyterLab ou Jupyter Notebook. Os dados brutos devem ser obtidos diretamente no portal do INEP. Certifique-se de ter as bibliotecas listadas acima instaladas.
