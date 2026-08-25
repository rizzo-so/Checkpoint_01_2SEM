# Checkpoint_01_2SEM
Integrantes:
- Enrico Giacometti
- Fernanda Botejara 
- Marcos Vinícius 
- Sofia Rizzo


Avaliação Prática — Computational Thinking of Engineering
 
  Objetivo do Projeto
O objetivo principal desta avaliação é demonstrar o domínio sobre **estruturas de dados em Python** (Listas, Tuplas e Dicionários) aplicadas ao consumo de dados reais provenientes de **APIs REST públicas**.
 
  Tecnologias e Conceitos Aplicados
- **Linguagem:** Python 3
- **Estruturas de Dados:** `list`, `tuple`, `dict`
- **Requisições HTTP:** Biblioteca `requests`
- **APIs Utilizadas:**
  - [AwesomeAPI](https://docs.awesomeapi.com.br/api-de-moedas) (Cotações de Moedas)
  - [OpenWeather API](https://openweathermap.org/api) (Dados Meteorológicos)
- **Ambiente:** Google Colab (Uso de *Secrets* para chaves de API)
 
  Estrutura da Avaliação
 
A atividade é dividida em duas situações-problema baseadas em cenários reais da engenharia mecatrônica:
 
Situação-problema 1: Custo de Protótipo Mecatrônico 
- **Descrição:** Uma equipe precisa estimar o custo de componentes importados (Sensores, Módulos, etc.) para um protótipo.
- **Tarefas:**
  - Extrair dados da AwesomeAPI (JSON aninhado).
  - Criar uma lista de tuplas contendo as moedas (USD, EUR, GBP) e seus valores de venda (`ask`).
  - Calcular o custo total em Reais (BRL) de uma lista de peças com base na cotação em tempo real.
 
Situação-problema 2: Condições para Teste de Campo 
- **Descrição:** O protótipo precisa ser testado em ambiente externo, sujeito a condições climáticas específicas de segurança.
- **Tarefas:**
  - Extrair dados da OpenWeather API para quatro cidades do estado de São Paulo.
  - Organizar os dados (Temperatura, Umidade e Velocidade do Vento) em uma lista de dicionários.
  - Criar um algoritmo de filtragem para aprovar cidades que atendam aos critérios:
    - Temperatura entre 18 °C e 32 °C.
    - Umidade $\le$ 85%.
    - Velocidade do vento $\le$ 10 m/s.
  - Gerar um relatório final de aprovação operacional.
 
Como Executar
 
1. Abra o arquivo Jupyter Notebook (`.ipynb`) no [Google Colab](https://colab.research.google.com/).
2. Na barra lateral esquerda do Colab, clique no ícone de **Secrets** (chave).
3. Adicione uma nova *secret* com o nome `OPENWEATHER_API_KEY` e insira a sua chave de acesso da API do OpenWeather no valor. Habilite o acesso da secret ao notebook.
4. Execute as células de requisição e conexão (disponibilizadas inicialmente no documento).
5. Execute as células com as respostas de cada questão.
