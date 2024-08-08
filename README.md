# Pesquisa de preços com Python 💸

### _Jetro Kepler, 2º Informática._ 💻

O projeto consiste em extração de informações de um site de forma automatizada (web scraping) com o objetivo de colocar os dados obtidos em uma planilha para a a verificação se certas operações devem ser realizadas.

Foram utilizadas as bibliotecas [_Selenium_](https://www.selenium.dev/documentation/) e [_Pandas_](https://pandas.pydata.org/docs/). O contexto é o seguinte:

> Trabalhamos em uma importadora e compramos e vendemos commodities:
> - Soja, Milho, Trigo, Petróleo, etc.

>Precisamos pegar na internet, de forma automática, a cotação de todas as commodites e ver se ela está abaixo do nosso preço ideal de compra. Se tiver, precisamos marcar como uma ação de compra para a equipe de operações.

Para realizar tal tarefa, o script pega em uma planilha da empresa (_commdities.xlsx_) quais produtos devem ser pesquisados e o preços que vão servir de parãmetro para a compra dos novos produtos.

Depois, o código abre o navegador, realiza a a pesquisa de preços e mostra o resultado em uma nova planilha (_commodities_atualizado.xlsx_), mostrando, agora, quais produtos devem ser comprados (_True_) ou não (_False_) de acordo com a a base de dados anterior.