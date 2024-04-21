# Started spliting the 4 sheets excel in 4 csv files separatedly.
Then i start EDA on the most important file, the dados_vendas.csv

### I Merged the two DataFrames 'dados_vendas' and 'info_loja' based on the column 'LOJA'
dados_vendas = pd.merge(dados_vendas, info_loja[['LOJA', 'FK_LOJA']], how='left', on='LOJA')

### Then i checked for Null Values, Missing Values and for outliers. I found some and i deal with them
