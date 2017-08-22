# Fixação da População Ocupada (FPO) na Região Metropolitana de São Paulo Segundo a Pesquisa OD-2007

### Autor: Vagner Sanches Vasconcelos (Agosto/2017)


## Resumo:
Na [Análise Exploratória dos Dados](http://nbviewer.jupyter.org/github/vsvasconcelos/EDA-R/blob/master/projecttemplatebr_vagner-rev4.html) da [Pesquisa Origem e Destino (Pesquisa O/D)](https://transparencia.metrosp.com.br/dataset/pesquisa-origem-e-destino/resource/dd9382bf-fbbe-4ca4-bd32-bf6150a59c4b) de 2007 na Região Metropolitana de São Paulo (RMSP) realizada pelo autor, chamou atenção a necessidade das 
pessoas deixarem sua zona de domicílio para trabalharem. Com este pano de fundo, essa visualização de dados apresenta o indicador Fixação da População Ocupada (FPO) - proposto por [Hiroi (2014)](http://www.aeamesp.org.br/biblioteca/stm/20smtf1410Tt11rl.pdf) -  que representa a porcentagem de população que ocupa empregos localizados na mesma zona de residência, em relação ao total de população ocupada residente nessa zona. Conforme Hiroi 2014), [...] quanto maior o FPO, melhor a adequação dos empregos locais à população ocupada residente,indicando melhor harmonia de determinado espaço no que se refere a distâncias e tempos de viagens entre locais de residência e trabalho".

## Design
A visualização é um [Mapa Coroplético](https://pt.wikipedia.org/wiki/Mapa_coropl%C3%A9tico) no qual quanto maior a tonalidade da cor azul maior é o FPO da zona; já para a cor amarela, quanto maior sua tonalidade menor é o FPO; as cores intermediárias são uma escala linear calculada em função do valor do FPO da respectiva zona.
O valor do FPO pode ser observado passando o cursor do mouse na zona de interesse. Também é possível utilizar o scroll do mouse para ampliar/diminuir o mapa.


## Feedback
### Questões Propostas:
1) O que você percebeu na visualização?

2) Que perguntas você tem sobre os dados?

3) Que relacionamentos você percebeu?

4) O que você acha que é o principal destaque dessa visualização?

5) Existe algo que você não entende no gráfico?

6) Outras observações/questões?

* 1: 
* 2:
* 3:

## Recursos

* [1 - Conversão shp para topjson](https://github.com/mbloch/mapshaper/issues/96)
* [2 - Projeções](https://wiki.osgeo.org/wiki/Brazilian_Coordinate_Reference_Systems)
* [3](https://medium.com/@aendrew/creating-topojson-using-d3-v4-10838d1a9538)
* [4](https://d3-geomap.github.io/docs/creating-topojson-files/)
* [5](https://stackoverflow.com/questions/17267248/)
* [6- ](how-where-do-i-get-geojson-data-for-states-provinces-and-administrative-region)
* [7 - Mapshaper](http://mapshaper.org/)
* [8 - tooltips](https://github.com/zeroviscosity/d3-js-step-by-step/blob/master/step-5-adding-tooltips.html)
* [9](http://alignedleft.com/tutorials/d3/)
* [10 - ](http://homepages.dcc.ufmg.br/~yussif/visdados/visbdgeod3js/desenvolvendomapas.html)
* [11 - ](https://github.com/jeanbauer/d3/wiki http://bl.ocks.org/michellechandra/0b2ce4923dc9b5809922)
* [12 - ](https://ben.balter.com/2013/06/26/how-to-convert-shapefiles-to-geojson-for-use-on-github/)
* [13 -](http://www.seithenin.com/d3.html)
* [14 - Mapa SP ](http://bl.ocks.org/helderdarocha/7d572d6e32266b932b4e4fabb3be7c08 (São Paulo))
* [15 - ](https://bl.ocks.org/almccon https://bost.ocks.org/mike/map/)