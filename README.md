# Bank Loan Risk Analysis
Analysis of customer data to enable bank loans, including bank data, personal data and motivation for the loan - Supervised classification (PT-BR)

## Objetivo
Conforme proposto pela IBM :
‘’O desafio consiste em criar um modelo de inteligência artificial capaz de realizar uma análise de risco para predizer se um empréstimo a um cliente deve ser feito ou não. Para isso, espera-se a utilização de um modelo de Machine Learning capaz de realizar uma classificação. O modelo pode ser desenvolvido na plataforma Watson Studio, e deve ser publicado em uma instância Watson Machine Learning. O modelo deverá ser treinado com os conjuntos de dados disponibilizado nesse repositório, contendo dados de clientes de bancos, como dados demográficos, sobre suas contas e sobre o empréstimo que querem realizar.’’

## Resumo do desenvolvimento

Dados acessados e coletados via ferramenta da IBM e incluso no jupyter notebook com a biblioteca Pandas, criando data frame especifico para cada vertente, dados pessoais, dados bancários e dados de empréstimo, após verificação todos os dados foram unidos em único dataframe e tratados para iniciar a analise exploratória tanto univariavel como bivariavel, observando o impacto na variável resposta. Em sequencia os dados foram preparados para serem utilizados no modelo de aprendizado de maquina, separados em conjuntos de teste e treino, treinados em 5 modelos (regressão logística, Classificador por Arvore de decisão, naive bayes,  clusterizaçao por vizinhos ou KNN e SVC), realizando o teste com uma semente aleatória única e dando resposta baseado no fator F1, o modelo svc apresentou o melhor resultado sendo este testado novamente para aprimorar seus parâmetros. Por fim com o modelo escolhido ele e aplicado a tabela resposta finalizando o desafio.

## Conclusão
Por fazer parte da maratona Behind the code 2021 o tempo de desenvolvimento do projeto foi bem curto, sendo feito em apenas 2 dias, e com foco direto na performance do modelo, fiquei satisfeito com o resultado podendo passar pelo primeiro ciclo de desenvolvimento do projeto com uma boa resposta.
Em vista do negocio quanto maior o valor de confiança do modelo(F1), teremos maiores certezas quanto a liberação de credito ao cliente, assim diminuindo o risco de não pagamentos e também agregando os clientes desejados, aqueles que pagam seus empréstimos, com essa informação e possível criar produtos mais atrativos a determinados públicos com menor risco a empresa (não pagadores ou falsos positivos) e aumentando sua base ‘boa’ de clientes (pagadores ou verdadeiros positivos).
