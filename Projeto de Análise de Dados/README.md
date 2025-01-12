# Projeto de Análise de Dados com Python - Bootcamp Hashtag Treinamentos

Este projeto foi desenvolvido como parte do bootcamp  da Hashtag Treinamentos, utilizando Python e bibliotecas como `pandas` e `plotly` para analisar dados relacionados a cancelamentos de contratos. O projeto é estruturado em blocos executáveis em um notebook Jupyter (`.ipynb`), permitindo a execução e visualização de resultados em cada etapa do processo.

## Funcionalidades

1. **Leitura e Visualização dos Dados**:
   - Carregamento dos dados a partir de um arquivo CSV (`cancelamentos.csv`).
   - Remoção da coluna `CustomerID`, que não é relevante para a análise.
   - Exibição das primeiras informações sobre a tabela e tratamento de dados ausentes.

2. **Análise Inicial**:
   - Verificação das distribuições dos dados e proporções de cancelamentos.
   - Uso do método `value_counts()` para calcular frequências absolutas e relativas.

3. **Visualização de Dados**:
   - Criação de gráficos interativos usando `plotly.express` para explorar a relação entre as variáveis e o status de cancelamento.

4. **Filtragem Avançada**:
   - Exclusão de registros com contratos mensais, alto número de ligações ao call center e atrasos significativos.
   - Reavaliação das distribuições após as filtragens.

## Pré-requisitos

Certifique-se de que o ambiente está configurado corretamente antes de executar o notebook:

- **Python 3.7+** instalado.
- Jupyter Notebook ou Jupyter Lab configurado.
- As bibliotecas Python necessárias:
  ```bash
  pip install pandas plotly
  ```
- Um arquivo `cancelamentos.csv` contendo os dados a serem analisados.

## Como Usar

1. **Abra o Notebook**:
   - Certifique-se de que o arquivo `.ipynb` está no mesmo diretório que o arquivo `cancelamentos.csv`.
   - Abra o notebook em seu ambiente Jupyter.

2. **Execute os Blocos**:
   - Execute os blocos sequencialmente para entender como cada etapa do processo funciona.
   - Analise os gráficos interativos e resultados exibidos para cada etapa.

3. **Interprete os Resultados**:
   - Verifique as proporções de cancelamentos antes e depois das filtragens.
   - Use os gráficos para identificar padrões nos dados.

## Estrutura do Notebook

1. **Leitura e Pré-processamento**:
   - Carregamento dos dados e exclusão de colunas irrelevantes.
   - Tratamento de valores ausentes.
2. **Análise Exploratória**:
   - Verificação de distribuições e frequências.
3. **Visualização com Gráficos**:
   - Gráficos de histograma para cada coluna, categorizados por status de cancelamento.
4. **Filtragem Avançada**:
   - Aplicação de filtros específicos para refinar os dados analisados.
5. **Reanálise Após Filtragem**:
   - Comparação das proporções antes e depois dos filtros.

## Detalhes Técnicos

- **Gráficos com Plotly**: Gera gráficos interativos para análise visual detalhada.
- **Filtragem Condicional**: Usa operações do `pandas` para excluir registros com valores indesejados.

## Personalização

- **Arquivo de Dados**: Substitua `cancelamentos.csv` por outro arquivo para analisar diferentes conjuntos de dados.
- **Filtros**: Ajuste as condições de filtragem conforme necessário para atender a requisitos específicos.

## Atenção

- **Consistência dos Dados**: Certifique-se de que os dados no arquivo CSV estão no formato esperado para evitar erros.
- **Requisitos de Gráficos**: Os gráficos interativos exigem que você visualize os resultados em um ambiente que suporte visualização HTML, como Jupyter.
