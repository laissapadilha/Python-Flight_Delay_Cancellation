# Análise dos voos domésticos nos Estados Unidos

**Fonte dos Dados:** [Flight Delay and Cancellation Dataset (2019-2023)](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023/data?select=flights_sample_3m.csv)

## Introdução

A base apresenta dados obtidos no site do Departamento de Transportes dos EUA e, contém informações sobre voos domésticos realizados entre janeiro de 2019 e agosto de 2023, como data do voo, cidade de origem e destino, cia aérea, duração do voo, tempo de atraso na partida/chegada, cancelamento, entre outras.

Através desta análise exploratória, buscou-se avaliar os seguintes aspectos:

- Quantidade de voos por mês ao longo do período analisado;
- Segmentação da quantidade de voos por cia aérea;
- Performance dos voos ao longo dos anos, considerando voos pontuais, adiantados, atrasados e cancelados;
- Performance dos voos segmentada por cia aérea;
- Rotas (cidade de origem/destino);
- Principais motivos do atraso de vos;

**A análise completa em Python pode ser acessada** [aqui](https://github.com/laissapadilha/Python-Flight_Delay_Cancellation/blob/b425a0b32c9fb60608cb6b79390f0cff11f5b933/Flights_Cancel_Delay.ipynb)

## Conclusão

Ao analisarmos a quantidade de voos ao longo do período estudado, observa-se que a pandemia da Covid-19 causou um impacto significativo no volume de voos. Em março de 2020, mais de 66 mil voos foram realizados, mas esse número caiu drasticamente para cerca de 18 mil em maio. A recuperação foi gradual, com a quantidade de voos permanecendo abaixo dos níveis de 2019 até maio de 2021, quando finalmente superou a marca de 50 mil voos mensais.

Em relação às companhias aéreas, as cinco que mais realizaram voos durante o período analisado foram a Southwest Airlines Co, Delta Airlines Inc, American Airlines Inc, SkyWest Airlines Inc e United Airlines Inc. A Southwest Airlines, primeira colocada do ranking, superou a segunda colocada em cerca de 180 mil voos, totalizando mais de 577 mil voos.

Ao avaliar a performance das companhias aéreas, podemos destacar os seguintes pontos:

- O percentual de pontualidade foi relativamente baixo, com a Southwest Airlines Co apresentando o maior índice, de apenas 6,67%;
- Observou-se um elevado percentual de voos que partiram adiantados, variando entre 44% e 75%;
- A média de antecipação dos voos foi inferior a 6 minutos, com um desvio padrão de apenas 3,34 minutos, o que indica que, apesar do alto percentual de voos adiantados, o tempo de antecipação foi, de maneira geral, curto;
- O percentual de voos atrasados variou entre 19% e 46%, sendo a Southwest Airlines Co a que apresentou o maior percentual;
- Os percentuais de cancelamento variaram entre 1,21% e 5,57%;
- Curiosamente, a Southwest Airlines Co foi a única entre as 5 maiores companhias em número de voos a figurar também entre as top 5 em termos de voos atrasados e cancelados;
- Em relação aos atrasos, 75,75% dos voos sofreram atrasos de até 1 hora, com 10,89% apresentando atrasos entre 1 e 2 horas;
- A média de atraso foi de 39,53 minutos, enquanto a mediana foi de 17 minutos, indicando uma distribuição assimétrica nos tempos de atraso;
- Embora a Southwest tenha liderado em termos de percentual de atraso, ficou em penúltimo lugar no que diz respeito à média de tempo de atraso (26,47 minutos);
- Ao observar a performance ao longo dos anos, nota-se que os percentuais de pontualidade, atraso e cancelamento se mantiveram estáveis, com exceção do ano de 2020, que foi marcado pelo pico da pandemia de Covid-19.

A base de dados abrange voos com origem ou destino em 373 cidades dos Estados Unidos, com as 10 principais sendo Chicago/IL, Atlanta/GA, Dallas/Fort Worth/TX, Denver/CO, New York/NY, Charlotte/NC, Houston/TX, Los Angeles/CA, Washington/DC e Phoenix/AZ. Exceto por Dallas/Fort Worth e Washington DC, todas as outras cidades estão entre as maiores de seus respectivos estados.

Analisando as 10 rotas com mais voos atrasados e cancelados, os seguintes pontos chamam atenção:

- New York aparece frequentemente como cidade de origem e destino em rotas com grandes volumes de atrasos e cancelamentos, destacando-se em quatro rotas de voos atrasados e em três rotas de voos cancelados;
- Chicago também aparece como cidade de origem e destino em várias rotas, com destaque para a Chicago x New York, que é a rota com mais atrasos, e a New York x Chicago, que é a que mais sofre com cancelamentos.

Por fim, ao analisar as correlações entre os motivos de atraso, observa-se que:

- Existe uma forte correlação entre o atraso na partida e na chegada, indicando que um voo atrasado na partida tende a sofrer atrasos também na chegada;
- A correlação entre o atraso causado pela companhia aérea e os atrasos na partida e na chegada é alta;
- O atraso decorrente da aeronave atrasada tem uma correlação moderada com o atraso na partida.

Os dados analisados forneceram uma visão detalhada sobre o desempenho das companhias aéreas e das rotas mais afetadas ao longo do período avaliado, além de oferecer insights valiosos sobre os fatores que podem influenciar os atrasos e cancelamentos.

