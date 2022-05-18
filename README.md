# 1º Challenge de Data Science da Alura
alurachallengedatascience1

## Sobre o desafio:
Este desafio simula a análise de dados dos clientes do AluraVoz, onde será necessário aplicar técnicas de DataScience para auxiliar o time de vendas a buscar estratégias para redução do Churn de clientes.

Ferramenta de gestão do projeto: trello , https://trello.com/b/pcPj8t1B/challenge-alura-week-1

### Semana 1: Primeiros passos em Data Science - limpeza dos dados trazidos de uma API
Principais atividades realizadas: 
- Leitura dos dados: formato json fonte http;
- Normalização de colunas: cada coluna possui um dicionário com dados embutidos, assim, cada uma das colunas foi normalizada usando 'json_normalize'.
- Concantenação: as colunas normalizadas foram concatenadas para formas o DataFrame 'dados_api'
- Análise de inconsistência nos dados: foi observado que as colunas 'Churn' e 'Charges Total' possuiam valores em branco. Para isso utilizou-se o df.info() e df.describe(). No entanto ao utilizar a função isnull() não aparecia dados nulos para tais colunas. Solução: utilizando o unique() foi possível identificar qual a str que estava constando nos campos sem valor e assim através da função replace() substituí-los por np.nan. 
Foi aplicado o dropna() para ambos Churn e Charges Total e as linhas com campos nulos nessas colunas foram removidas do dataframe; que agora é a cópia: dados_new.
- Tradução das colunas: foram traduzidos os nomes das colunas e os valores de alguns campos que estavam em inglês. Não foi aplicado uma função, portanto, foi feita uma tradução por vez.
- Criação da coluna tempo_dias: esta coluna foi calculada através da divisão do valor da coluna 'tenure' por 30, uma vez que a coluna 'tenure' está em meses. Logo podemos analisar o tempo de contrato em dias.


### Semana 2: Explorando os dados - vendo as informações por uma outra perspectiva


### Semana 3
### Semana 4
