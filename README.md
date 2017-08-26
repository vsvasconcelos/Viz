## Fixação da População Ocupada (FPO) na Região Metropolitana de São Paulo Segundo a Pesquisa OD-2007

### Autor: Vagner Sanches Vasconcelos (Agosto/2017)

## Resumo:
Na [Análise Exploratória dos Dados](http://nbviewer.jupyter.org/github/vsvasconcelos/EDA-R/blob/master/projecttemplatebr_vagner-rev4.html) da [Pesquisa Origem e Destino (Pesquisa O/D)](https://transparencia.metrosp.com.br/dataset/pesquisa-origem-e-destino/resource/dd9382bf-fbbe-4ca4-bd32-bf6150a59c4b) de 2007 na Região Metropolitana de São Paulo (RMSP) realizada pelo autor, chamou atenção a necessidade das 
pessoas deixarem sua zona de domicílio para trabalharem. Com este pano de fundo, essa visualização de dados apresenta o indicador Fixação da População Ocupada (FPO) - proposto por [Hiroi (2014)](http://www.aeamesp.org.br/biblioteca/stm/20smtf1410Tt11rl.pdf) -  que representa a porcentagem de população que ocupa empregos localizados na mesma zona de residência, em relação ao total de população ocupada residente nessa zona. Conforme Hiroi 2014), [...] quanto maior o FPO, melhor a adequação dos empregos locais à população ocupada residente,indicando melhor harmonia de determinado espaço no que se refere a distâncias e tempos de viagens entre locais de residência e trabalho".

## Design
A visualização é um [Mapa Coroplético](https://pt.wikipedia.org/wiki/Mapa_coropl%C3%A9tico) no qual quanto maior a tonalidade da cor azul maior é o FPO da zona; já para a cor amarela, quanto maior sua tonalidade menor é o FPO; as cores intermediárias são uma escala linear calculada em função do valor do FPO da respectiva zona.
O valor do FPO pode ser observado passando o cursor do mouse na zona de interesse. Também é possível utilizar o scroll do mouse para ampliar/diminuir o mapa.
Destaque especial para o site [mapstater](http://mapstarter.com/) que possui várias funcionalidade que ajudam no desenvolvimento de visualizações com mapas.

## Feedbacks

### Feedback Avaliador A - 1ª versão:
1A) O que você percebeu na visualização?
<span style="color:green">Resp.: As regiões mais afastadas parecem ter mais fixação, porém, por serem muito maiores não quer dizer que o deslocamento não é grande...</span>.

2A) Que perguntas você tem sobre os dados?
<span style="color:green">Resp.: Por que tantos indefinidos? Os dados são referentes a que mora e trabalha na mesma região, certo? Mas tem regiões muito pequenas e outras muito grandes. Talvez valesse a pena fazer ou dar a opção de visualização por distância percorrida. Acho que mudaria bastante o resultado apresentado, principalmente nas regiões próximas ao centro...</span>

3A) Que relacionamentos você percebeu?
<span style="color:green">Resp.: Tirando alguns casos, como Marsilac, Itapeti, Reservatório de Mogi, Luz e Pq Dom Pedro, as regiões grandes tem maior FPO e regiões pequenas tem baixo FPO.
Pode ser interessante colocar as principais vias de acesso, para perceber o porque de algumas conclusões, como o isolamento da região de Salesópolis, Pirapora e Juquitiba (esta tem a Regis, mas é único acesso).</span>

4A) O que você acha que é o principal destaque dessa visualização?
<span style="color:green">Resp.: A interatividade: ver os dados ao passar o mouse e o zoom.</span>

5A) Existe algo que você não entende no gráfico?
<span style="color:green">Resp.: Não</span>

6A) Outras observações/questões?
<span style="color:green">Resp.: Não</span>

### Feedback Avaliador B - 1ª versão:
1B) No código (arquivo html), mesmo sendo comentários, é importante tentar deixar estas linhas com no máximo uns 80 a 100 caracteres.
Padronizar os comentários em Português e citar nas seções de resumo ou design eventuais códigos base que tenham sido utilizados neste trabalho.
2B) Acrescentar título e legenda.
3B) Por quê os dados estão sendo apresentados na forma de um mapa, e não em um outro tipo de gráfico, como por exemplo um gráfico de barras?
4B) Há algum motivo em especial para termos usado uma escala entre azul e amarelo?
5B) Escrever um pouco mais sobre mapas coropléticos e sua função.

### Feedback Avaliador C - 1ª versão:
1C) Seria interessante se o mapa você do tipo "Google Maps".

Modificações Realizadas conforme Feedbacks.
1B) Revisado o código.
2B) Acrescentado título e legenda.
3B) e 5B) Foi utilizado a apresentação por meio de mapa para propiciar contexto espacial aos dados, neste sentido o mapa Coroplético foi adotado pois apresenta uma forma rápida de comparação entre as zonas.
4B) As cores adotadas (azul e amarelo) foram escolhidas após varias outras terem sido testadas; optou-se em não utilizar vermelho e verde devido a pessoas com problema de deltonismo terem dificuldades de visualizá-las.


Modificações não implementadas.
1A) Na pesquisa OD as regiões mais afastadas do centro de SP são mais agregadas, isto é, possuem menos zonas,
com isto, realmente o FPO pode ser alto, mas o trabalhador pode demorar muito tempo para chegar ao trabalho.
Para trabalhos futuros, o indicador Tempo Médio de Deslocamento (TMD) pode ser testado.
2A) O dados indefinidos são devidos a ausência destes na Pesquisa OD/2007. Quanto a sugestão da distância, acredito que o tempo
(TMD) possa ser uma variável melhor, uma vez que pode haver uma pequena distância, mas com um tempo de chegada demorado.
3A) e 1C) Para trabalhos futuros tentaremos utilizar mapas tipo "Google Maps", como [este](http://bl.ocks.org/anonymous/raw/8d85645022e027b1eaffb88d286e6b97/), resultante do Topojson.json utilizado neste trabalho e carregado no site [geojson.io](http://geojson.io/#map=9/-23.6247/-46.4518).

## Recursos

* [1 - Conversão de shp para TopoJson](https://github.com/mbloch/mapshaper/issues/96)
* [2 - Projeções](https://wiki.osgeo.org/wiki/Brazilian_Coordinate_Reference_Systems)
* [3 - Inspiração](https://medium.com/@aendrew/creating-topojson-using-d3-v4-10838d1a9538)
* [4 - Criando arquivos TopoJson](https://d3-geomap.github.io/docs/creating-topojson-files/)
* [5 - Conversão](https://stackoverflow.com/questions/17267248/)
* [6 - Conversão de formato de mapas](how-where-do-i-get-geojson-data-for-states-provinces-and-administrative-region)
* [7 - Visualização de TopoJson - Mapshaper](http://mapshaper.org/)
* [8 - Tooltips](https://github.com/zeroviscosity/d3-js-step-by-step/blob/master/step-5-adding-tooltips.html)
* [9 - Scott Murray](http://alignedleft.com/tutorials/d3/)
* [10 - Tutorial PT_BR](http://homepages.dcc.ufmg.br/~yussif/visdados/visbdgeod3js/desenvolvendomapas.html)
* [11 - Documentação Biblioteca D3.js](https://github.com/jeanbauer/d3/wiki)
* [12 - Conversão shp2json](https://ben.balter.com/2013/06/26/how-to-convert-shapefiles-to-geojson-for-use-on-github)
* [13 - Conversão](http://www.seithenin.com/d3.html)
* [14 - Mapa SP ](http://bl.ocks.org/helderdarocha/7d572d6e32266b932b4e4fabb3be7c08 (São Paulo))
* [15 - Exemplos](https://bl.ocks.org/almccon)
* [16 - Inspiração](http://bl.ocks.org/michellechandra/0b2ce4923dc9b5809922)
* [17 - Tutorial](https://bost.ocks.org/mike/map/)