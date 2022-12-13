## US_house_price_analysis 
  Status do projeto (em andamento)

## Objetivo
  O objetivo desse projeto é analisar o relacionamento entre índices financeiros e o preço de imóveis nos Estados Unidos. Os dados foram extraidos através da API FRED (dados econômicos do Federal Reserve Bank of St. Louis).
    
## Técnicas
  - Extração
  - Limpeza e Processamento
  - Visualização
  - Exportação
  
## Etapas
  - No site https://research.stlouisfed.org/ pesquisei e identifiquei os dados que pudessem me ajudar a descobrir os índices cuja variação tem maior correlação com o índice dos preços dos imóveis nos Estados Unidos.
 - Filtrei os dados do S&P 500 para converter informações diárias em mensais e poder comparar com os índices que tem informação mensal. Fiz o mesmo processo com a taxa de juros.
 - Juntei todas as informações em um único dataframe.
 - Usei MinMaxScaler para normalizar os valores que foram utilizados nos gráficos.
 - Exportei os dados para o banco de dados no MySQL.
 - Fiz envio automático de e-mail com informações diárias.
 - Gerei arquivo de log.


## Ferramentas
* Python
  * Jupyter notebook
  * datetime
  * dotenv
  * email
  * fredapi
  * logging
  * matplotlib
  * numpy
  * os
  * pandas
  * plotly
  * pretty_html_table
  * pymysql
  * seaborn
  * sklearn
  * smtplib
  * sqlalchemy
  
## Conclusão
 - Observei que nos últimos 10 anos a evolução do índice de preço dos imóveis acompanhou a evolução do S&P 500 (um dos principais indicadores de ações norte-americanas, seria equivalente ao Ibovespa aqui no Brasil).

![image](https://user-images.githubusercontent.com/112282677/207201190-ae5bfa80-a3b3-45b2-9c9e-ca70c812983b.png)

 - Inflação e Taxa de Juros não apresentaram impacto expressivo no preço dos imóveis. Porém, vale ressaltar que a inflação alta observada a partir do segundo semestre de 2021 nos EUA é uma situação atípica no país, sendo recomendável continuar essa análise nos próximos meses para verificar se o padrão recente se mantém. 
 
 ![image](https://user-images.githubusercontent.com/112282677/207202351-37e8ba32-6a52-4d34-adb6-0f04a8a18bb0.png)

![image](https://user-images.githubusercontent.com/112282677/207202414-859dcf3a-be5f-4f69-bdb2-eb485f36a9aa.png)

 - Exceto pelo pico de desemprego em 2020, o comportamento está dentro do esperado. Desemprego baixo, preço dos imóveis mais alto, desemprego alto, preço dos imóveis mais baixo. Essa relação é bem visível no gráfico entre 2013 e 2019.
 
 ![image](https://user-images.githubusercontent.com/112282677/207202975-c54ef846-41c9-49f6-9011-7680b57f3498.png)
 
   - Essa foi uma análise introdutória para obter alguns insights. Como próximos passos, poderíamos, por exemplo, segmentar por regiões e verificar se o comportamento foi igual em todo o país.


📫 Se você tiver algum comentário ou sugestão, por favor me avise!
    
    https://www.linkedin.com/in/lenagrumbach/
    
    lenagrumbach@gmail.com

