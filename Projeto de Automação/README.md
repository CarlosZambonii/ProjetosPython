# Projeto de Automação Python - Bootcamp Hashtag Treinamentos

Este projeto foi desenvolvido como parte do bootcamp  da Hashtag Treinamentos, utilizando Python e bibliotecas como `pyautogui`, `time` e `pandas` para automatizar tarefas repetitivas e melhorar a produtividade.

## Funcionalidades

1. **Acesso Automático ao Sistema**:
   - Abre o navegador Google Chrome.
   - Navega até a página de login.
   - Realiza login com credenciais fornecidas.

2. **Leitura de Dados de um Arquivo CSV**:
   - Lê dados de um arquivo `produtos.csv` que contém informações sobre produtos.

3. **Automação de Cadastro**:
   - Insere os dados do arquivo CSV (código, marca, tipo, categoria, preço unitário, custo e observações) em um sistema.
   - Realiza as interações no sistema de forma automatizada, preenchendo os campos e enviando os dados.

## Pré-requisitos

Certifique-se de que o ambiente está configurado corretamente antes de executar o script:

- **Python 3.7+** instalado.
- As bibliotecas Python necessárias:
  ```bash
  pip install pyautogui pandas
  ```
- Um arquivo `produtos.csv` contendo os dados no seguinte formato:
  ```csv
  codigo,marca,tipo,categoria,preco_unitario,custo,obs
  ```

## Como Usar

1. **Baixe e Configure o Projeto**:
   - Clone este repositório ou baixe os arquivos.
   - Certifique-se de que o arquivo `produtos.csv` está no mesmo diretório do script.

2. **Execute o Script**:
   - Inicie o script no terminal:
     ```bash
     python automacao.py
     ```

3. **Interaja com o Script**:
   - O script controlará automaticamente o mouse e teclado para interagir com o sistema.

## Detalhes Técnicos

- **`pyautogui.PAUSE`**: Define um pequeno intervalo entre os comandos para evitar problemas com a velocidade da automação.
- **Coordenações de Clique**: As coordenadas de clique no sistema são configuradas para uma resolução de tela específica. Certifique-se de ajustá-las caso sua resolução seja diferente.
- **Leitura de CSV**: Utiliza a biblioteca `pandas` para manipular os dados de forma eficiente.

## Personalização

- **Credenciais de Login**: Altere o e-mail e senha no script para utilizar suas credenciais.
- **Coordenadas do Mouse**: Utilize o comando `pyautogui.position()` para capturar coordenadas específicas do seu sistema e ajuste os valores de `x` e `y` no código.

