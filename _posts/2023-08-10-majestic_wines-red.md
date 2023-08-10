---
title: 'Majestic wines red wine analysis'
date: 2023-08-10
permalink: /posts/2023/2-majestic_wines-red

---

I present some analysis of red wines available on [Majestic wines](https://www.majestic.co.uk), with data obtained using my recently released [chrome extension](https://chrome.google.com/webstore/detail/majestic%2Bvivino/neohjloinpdpfddkjfcagikdgepjbmee). 

The dataset is limited to currently in stock red wines on [Majestic wines](https://www.majestic.co.uk). Half bottles, port, wines with a price over £100 or wines without Vivino ratings were removed from the dataset. Only countries with more than 10 wine were included in the dataset, therefore excluding: Austria, England, Georgia, Germany, Greece, Hungary, Israel, Lebanon, Moldova, Romania and Slovenia.

| Country      | Number of wines | Number of Regions | Average price / £ | Average rating |
| -----------      | ----------- | ----------- | -----------| ----------- |
| France      | 114       |  68       | 20.3       |3.8       |
| Spain      | 52       |  22       | 14.3       |3.9       |
| Italy      | 50       |  24       | 15.3       |3.8       |
| Australia      | 39       |  9       | 17.0       |3.9      |
| South Africa      | 31       |  9       | 13.8       |3.8      |
| Chile      | 23       |  11       | 10.9       |3.7       |
| Argentina      | 22       |  2       | 12.4       |3.9       |
| USA      | 18       |  12       | 19.3       |3.9       |
| Portugal      | 13       |  8       | 13.4       |3.8       |
| New Zealand      | 11       |  4       | 15.4       |3.7       |

As expected France has not only the most wines and the most wine regions, but also the highest average price. Surprisingly, the average rating of 3.81 is lower than many other countries including Spain and Italy. This may suggest a strong hierarchy in the quality of French wines, or that French wines are reviewed more harshly. It seems likely that the reviewers of high end French wines are more critical than the reviewers of low end Italian wines, introducing an asymmetry in the rating system.

<img src="https://github.com/chrisahart/vivino-majestic/blob/main/analysis/plots/wine_red/price_rating_all.png" style="display: block; margin: auto;" />

This figure shows the Vivino rating and Majestic Wines price for all wines, coloured by country, showing a strong correlation between Vivino rating and Majestic Wines price. 

<img src="https://github.com/chrisahart/vivino-majestic/blob/main/analysis/plots/wine_red/price_rating_france-multiple-regions-only.png" style="display: block; margin: auto;" />

This figure shows the Vivino rating and Majestic Wines price for wines in France, coloured by region, showing a strong correlation between Vivino rating and Majestic Wines price. As there are 68 wine regions in the database for France, only regions with more than 1 wine are represented. 'Vin de France, 'Côtes-du-Rhône' and 'Beaujolais' appear to be the wine regions with the greatest value. Notably, 'St Emilion Grand Cru' also appears to provide surprisingly good value.

| Product Name      | Rating | Price / £ | Region| Country|
|-----------|-----------|-----------|-----------|-----------|
The Guvnor |4.0|6.99|Valdepeñas|Spain
Ramn Bilbao Seleccin Especial |4.2|8.99|Rioja|Spain
The Guvnor VIP |4.0|9.99|Vino de España|Spain
Olarra Clsico Rioja Reserva |4.0|11.99|Rioja|Spain
Definition Rioja Reserva |4.0|12.99|Rioja|Spain
Marqus de Cceres  Reserva |4.0|13.99|Rioja|Spain
Bodega Matsu El Recio Toro|4.1|13.99|Toro|Spain
Chozas Carrascal Anma |4.0|13.99|Utiel-Requena|Spain
Marqus de Riscal Rioja Reserva|4.0|14.99|Rioja|Spain
Beronia Rioja Reserva|4.0|15.99|Rioja|Spain
Bodegas Bardos Ribera del Duero Reserva|4.1|15.99|Ribera del Duero|Spain
Cune Rioja Gran Reserva|4.0|17.99|Rioja|Spain
Marqus de Cceres Rioja Gran Reserva |4.1|19.99|Rioja|Spain
Muga Rioja Reserva |4.2|19.99|Rioja|Spain
Primo Rosso Appassimento |4.1|8.99|Puglia|Italy
Negrar Appassimento |4.1|9.99|Veneto|Italy
Pasqua 'Desire, Lush & Zin' Primitivo|4.2|9.99|Puglia|Italy
Polvanera 'P24' Primitivo |4.0|13.99|Gioia del Colle|Italy
Domini Veneti La Casetta Valpolicella Ripasso |4.2|15.99|Valpolicella Ripasso|Italy
Fidora Valpolicella Ripasso |4.0|16.99|Valpolicella Ripasso|Italy
Antica Vigna Amarone della Valpolicella|4.0|17.99|Amarone della Valpolicella|Italy
Definition Barolo |4.2|18.99|Barolo|Italy
Barista Pinotage 202122 Western Cape|4.1|8.99|Western Cape|South Africa
Iona The Good Stuff |4.1|10.99|Cape South Coast|South Africa
Capaia One 201819 Tygerberg|4.0|12.99|Western Cape|South Africa
Rustenberg John X Merriman |4.0|16.99|Stellenbosch|South Africa
Morgenster Lourens River Valley |4.2|17.99|Stellenbosch|South Africa
Radford Dale Antithesis Syrah|4.1|18.99|Stellenbosch|South Africa
Rupert Rothschild Classique |4.0|18.99|Western Cape|South Africa
Marcelo Pelleriti Malbec |4.1|9.99|Mendoza|Argentina
Vialba Reserve Malbec |4.1|10.99|Mendoza|Argentina
Catena Malbec |4.0|12.99|Mendoza|Argentina
Vialba Gran Reservado Malbec |4.0|16.99|Mendoza|Argentina
Terrazas de los Andes Malbec |4.2|16.99|Mendoza|Argentina
Mendel Selection Malbec |4.0|19.99|Mendoza|Argentina
19 Crimes Red Blend |4.0|8.99|Victoria|Australia
Casella PepperBox Shiraz |4.0|9.99|South Eastern Australia|Australia
Two Hands Angels Share Shiraz | 4.0|18.99|McLaren Vale|Australia
Two Hands Gnarly Dudes Shiraz |4.0|18.99|Barossa Valley|Australia
Two Hands Sexy Beast Cabernet Sauvignon |4.0|18.99|McLaren Vale|Australia
Toast Honey Pinot Noir |4.0|12.99|Lodi|USA
Bread Butter Cabernet Sauvignon |4.0|13.99|California|USA
Bread Butter Pinot Noir |4.0|13.99|Napa Valley|USA
3 Finger Jack Zinfandel |4.1|14.99|Lodi|USA
Luis Felipe Edwards 900 Single Vineyard |4.0|14.99|Colchagua Valley|Chile
Santa Rita Triple C |4.1|15.99|Maipo Valley|Chile
Managers Choice VIK A Cabernet Sauvignon |4.2|16.99|Cachapoal Valley|Chile
Chteau dAngls Grand Vin |4.1|15.99|La Clape|France
Alain Jaume Les Champauvins |4.0|15.99|Côtes-du-Rhône|French
Villa Maria Reserve  |4.0|17.99|Hawke's Bay|New Zealand

This table contains all wines with a Vivino rating above 4.0 and a price below £20, representing the greatest value. Wines are shown in price ascending order, grouped by country of descening number of wines. A [.csv file](https://github.com/chrisahart/vivino-majestic/blob/main/analysis/data/wine_red/wines_rating-above-4.0_price-below-20.csv) is available in the Github repository. This data indicates that Vivino users have a preference for smooth, low acidity, reasonably sweet fruit forward wines.
