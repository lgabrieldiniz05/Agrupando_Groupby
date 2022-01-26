# Agrupando_Groupby
<h2>Agrupando linhas de um DataFrame</h2>

<h3>Primeiro realizamos o import do pandas</h3>
<h5><i>import pandas as pd</i></h5>
<h3>Em seguida criamos uma variável tabela para receber o nosso arquivos xlsx</h3>
<h5><i>tabela = pd.read_excel('Vendas.xlsx')</i></h5>
<h3>E utilizando o comando display para imprimir nossa tabela na tela</h3>
<h5><i>display(tabela)</i></h5>
<div align="center"><img src="https://user-images.githubusercontent.com/90981124/151082684-d7d6dcd5-4e70-4a6c-bbaa-5cb01dbf4bc9.png" width="900px" /></div>

<h2>Utilizando Groupby</h2>
<h3>Para agrupar as linhas utilizamos o seguinde condigo</h3>
<h5><i>faturamento_loja = tabela[['ID Loja', 'Valor Final']].groupby('ID Loja').sum()</i></h5>
<h6>tabela[['ID Loja', 'Valor Final']] ->Para filtrar as colunas desejadas</h6>
<h6>.sum() ->Para somar os valores numéricos da coluna 'Valor Final'</h6>
<h3>E utilizamos o comando display para imprimir a nova tabela</h3>
<h5><i>display(faturamento_loja)</i></h5>
<div align="center"><img src="https://user-images.githubusercontent.com/90981124/151082731-1a7ca296-6446-41bb-acec-08dce6e7b194.png" width="900px" /></div>
