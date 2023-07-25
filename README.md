# analise_dados_churn

## Descrição

Este repositório apresenta a análise de churn na empresa PetLove&CO, a maior plataforma dedicada aos cuidados com animais de estimação na América Latina. O objetivo desse projeto é analisar os dados de churn, identificar padrões e insights relevantes, e fornecer recomendações de negócio para redução da taxa de cancelamento de assinaturas.

A equipe de Assinatura da PetLove&CO enfrenta o desafio de reduzir a perda de assinantes, ou seja, diminuir a taxa de churn. Neste case, abordaremos a análise dos dados dos últimos meses para identificar aprendizados e sugerir próximos passos.

## Status do projeto
Versão 1.0

## Tecnologias utilizadas
Python 3.9.13 | Bibliotecas: pandas, datetime e matplotlib

## Sobre os Arquivos

- `tratamento_inicial.ipynb`: Notebook Jupyter contendo o código-fonte utilizado para o tratamento inicial dos dados, incluindo limpeza, transformação e preparação dos dados para a análise.

- `analise_dados.ipynb`: Notebook Jupyter contendo o código-fonte utilizado para a análise exploratória dos dados, incluindo visualizações gráficas e conclusões importantes.

- Pasta `arquivos`: Pasta contendo os seguintes arquivos:
  - `data_bruta.csv`: Arquivo CSV com os dados brutos coletados inicialmente.
  - `data_tratada.parquet`: Arquivo Parquet contendo a base de dados gerada após o tratamento inicial.

- `relatorio.html`: Arquivo HTML contendo um relatório com as principais descobertas da análise de dados. Esse relatório é destinado a equipes externas e oferece uma visão geral dos insights e conclusões obtidos no projeto.

## Como usar

1. Clone o repositório em sua máquina local.
2. Certifique-se de ter as dependências instaladas. Caso não tenha, instale-as utilizando o gerenciador de pacotes pip.
3. Após a conclusão do scraping, execute o arquivo `analise_dados.ipynb` para realizar os tratamentos iniciais, selecionar as colunas que serão utilizadas na análise a seguir, e gerar a data_tratada.parquet
4. Utilize o arquivo `analise_dados.ipynb` para realizar a análise exploratória dos dados de churn
5. Leia o relatorio.html para obter insights sem se preocupar com linhas de código.

## Sobre os Dados

Os dados utilizados nesta análise foram disponibilizados pela equipe de Engenharia de Dados da PetLove&CO e estão armazenados no arquivo `data-test-analytics.csv`. As informações presentes no conjunto de dados incluem:

| Coluna             | Descrição                                                  |
|--------------------|------------------------------------------------------------|
| id                 | Identificação do cliente                                   |
| created_at         | Data de criação da assinatura                              |
| updated_at         | Data da última modificação da assinatura                   |
| deleted_at         | Data de cancelamento da assinatura                         |
| name_hash          | Nome do usuário (criptografado)                            |
| email_hash         | Email do usuário (criptografado)                           |
| address_hash       | Endereço do usuário (criptografado)                        |
| birth_date         | Data de aniversário do cliente                             |
| status             | Status da assinatura                                       |
| version            | Versão da assinatura                                       |
| city               | Cidade do cliente                                          |
| state              | Estado do cliente                                          |
| neighborhood       | Bairro do cliente                                          |
| last_date_purchase | Data do último pedido que ocorreu pela assinatura          |
| average_ticket     | Média de gasto por pedido                                  |
| items_quantity     | Média de itens na assinatura                               |
| all_revenue        | Total de receita realizado pelo cliente                    |
| all_orders         | Total de pedidos realizado pelo cliente                    |
| recency            | Tempo desde a última compra do cliente                     |
| marketing_source   | Canal de marketing que converteu a assinatura              |


## Resumo da Análise

Durante a análise de churn, foram identificados os seguintes aprendizados e insights importantes:

1. O churn vem crescendo ao longo dos anos, com destaque para os meses de dezembro, janeiro e fevereiro, que possuem as maiores quantidades de churn.

2. Versão: As versões 3 e 4 apresentam um maior número absoluto de cancelamentos, sugerindo que essas versões enfrentam desafios em relação à retenção de clientes. Apesar de, ao considerarmos a porcentagem de churn em relação ao total de assinantes de cada versão, notarmos que elas não possuem a maior porcentagem, elas ainda representam a parcela mais importante de assinaturas.

3. Canais de Marketing: Os canais "telegram_whatsapp" e "organic_search" possuem altas taxas de cancelamentos. Sugere-se uma revisão das estratégias de marketing para esses canais.

4. Faixa etária: A faixa etária "31-45" possui a maior quantidade de churn em relação ao total de assinantes, devendo ter uma atenção maior para reduzir a quantidade. Além disso, a faixa etária <31 possui a maior porcentagem de churn. Essa faixa etária representa um grupo de clientes que parece ser mais propenso a cancelar suas assinaturas, sendo importante entender o motivo por trás desse comportamento.

5. Estado: O estado "RS" apresenta a maior quantidade total de churns, além de que, junto com SE, possui a maior porcentagem de churn em relação ao total de assinantes. Clientes localizados nesse estado têm maior probabilidade de cancelar suas assinaturas. Portanto, é necessário realizar pesquisas e análises adicionais para compreender os motivos que levam os clientes dessa região a cancelarem suas assinaturas.


## Próximos Passos

1. Com base na análise realizada, algumas sugestões de próximos passos são:

2. Análise Comportamental: Realizar uma análise mais aprofundada do comportamento dos clientes que cancelaram suas assinaturas, buscando padrões ou eventos específicos que possam estar correlacionados com o churn.

3. Pesquisa de Satisfação: Realizar pesquisas de satisfação com os clientes que cancelaram suas assinaturas para entender os motivos por trás da decisão de cancelamento e obter feedback sobre a experiência com o serviço.

4. Campanhas de Retenção: Desenvolver campanhas de retenção de clientes, oferecendo benefícios exclusivos, descontos ou brindes para incentivar os clientes a manterem suas assinaturas ativas.

5. Melhorias nas Versões: Identificar possíveis melhorias nas versões 3 e 4 do serviço de assinatura para aumentar a satisfação e retenção dos clientes.

6. Personalização: Investir em estratégias de personalização, oferecendo recomendações de produtos e serviços com base no histórico de compras e preferências de cada cliente.

7. Monitoramento Contínuo: Estabelecer um processo de monitoramento contínuo do churn, analisando regularmente os dados para identificar mudanças de tendência e tomar ações proativas para reduzir o churn.

## Contato

Desenvolvedora do Projeto: Isabela Vitoriano

• Linkedin: [https://www.linkedin.com/in/isabela-vitoriano/](https://www.linkedin.com/in/isabela-vitoriano/)

• E-mail: [isabelavitoriano.ss@gmail.com](isabelavitoriano.ss@gmail.com)
