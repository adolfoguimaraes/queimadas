# Dados sobre queimadas 

Este repositório possui os dados que foram processados para gerar a visualização que está disponível [neste link](https://observablehq.com/@adolfoguimaraes/swd-challenge-fev-22?collection=@adolfoguimaraes/swd-challenge).

Os dados foram coletados diretamente da página: https://queimadas.dgi.inpe.br/queimadas/aq1km/. Como não tinha a possibilidade de extrair os dados diretamente do link, foram compiados os códigos html das tabelas que possuem as informações desejadas. Os htmls copiados estão na pasta [input/](input/dados_html).

Os dados possuem informações sobre a área (em km2) queimada em cada ano e mês de 2003 até 2021. Além disso, as tabelas possuem as informações separadas por bioma: Amazônia, Caatinga, Cerrado, Mata Atlântica, Pampa e Pantanal. 

Os htmls são processados e gerado um único arquivo com as informações desejadas. O arquivo de saída `br_queimadas_area_bioma.csv` está na pasta [output/](output/) e possui os seguintes campos:

* **ano:** Ano do dado coletado;
* **mes:** Mês (em inteiro) do dado caletado;
* **mes_nome:** Nome do mês correspondente ao campo `mes`;
* **bioma:** Nome do bioma do dado coletado;
* **total:** Total em km2 de área queimada;
* **total_acumulado:** Total acumulado por ano, mês e bioma.
