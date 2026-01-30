# Data Cleaning com Python & Pandas

## Sobre o Projeto

Este projeto foi desenvolvido como parte de uma atividade prática de Data Cleaning (Limpeza de Dados). O objetivo principal é transformar um conjunto de dados brutos em um dataset estruturado e confiável, pronto para processos futuros de Mineração de Dados e Análise Preditiva.

O projeto aborda problemas comuns em datasets reais, como:
* Valores ausentes (NaN).
* Formatos de data inconsistentes.
* Incorreções em tipos de variáveis.

### Tecnologias Utilizadas
* Linguagem: Python
* Biblioteca Principal: Pandas
* Ambiente: Jupyter Notebook / Google Colab

### O Processo de Limpeza (Pipeline)
O roteiro de tratamento seguiu as seguintes etapas críticas:
1. Carga e Inspeção
  * Leitura do arquivo CSV com atenção aos delimitadores (;).
  * Inspeção inicial das primeiras e últimas linhas para entender a estrutura dos dados.
2. Tratamento de Valores Nulos
  * Coluna 'Calories': Substituição de valores nulos por 0.
  * Coluna 'Date': Inicialmente preenchida com um valor sentinela (1900/01/01) e, posteriormente, tratada para evitar erros de processamento.
3. Padronização de Datas
  * Converter strings para objetos datetime.
  * Corrigir formatos sem separadores (ex: 20201226 para 2020/12/26).
  * Remoção final de registros que ainda permaneciam nulos após a tentativa de conversão.

### Estrutura do Conjunto de Dados
As colunas tratadas foram: | Coluna | Descrição | | :--- | :--- | | ID | Identificador único do registro | | Duration | Duração da atividade em minutos | | Date | Data da atividade (formato YYYY-MM-DD) | | Pulse | Batimentos cardíacos médios | | Maxpulse | Batimentos cardíacos máximos | | Calories | Calorias queimadas durante a atividade |

## Como executar

1. Clone o repositório:

> git clone https://github.com/seu-usuario/nome-do-repositorio.git

2. Instale as dependências:

> pip install pandas

3. Execute o script principal ou o notebook.
