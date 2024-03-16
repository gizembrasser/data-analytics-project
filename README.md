# Het eindproject - Gemeentelijke financiën Nijkerk

Link naar Github repository: https://github.com/gizembrasser/data-analytics-project/data-analytics-project/01-level

## Beschrijving
Dit dashboard weergeeft informatie over de gemeentelijke financiën van Nijkerk vergeleken met de rest van Nederlandse gemeenten. De data is afkomstig uit de begrotingen (2020 - 2024) en jaarrekeningen (2020 - 2022) van alle gemeenten, en uit bevolkingsgegevens van deze gemeenten. Het doel van het dashboard is om de volgende businessvragen te beantwoorden: 

1. Hoe groot is het verschil tussen het saldo van de begroting/jaarrekening in Nijkerk vergeleken met de rest van de gemeenten?
2. Hoeveel verdient de gemeente Nijkerk aan baten vergeleken met andere gemeenten?
3. Bewoners in Nijkerk vinden dat er opvalled veel leegstand is; hoe vergelijkt de grondexploitatie met de rest van de gemeenten?
4. Hoe vergelijkt de solvabiliteit van de gemeente Nijkerk met de rest van de gemeenten?
5. Zijn er financiële kengetallen die alarmbellen moeten gaan rinkelen bij de gemeente Nijkerk?

## Installatie-instructies
De datatransformatie is gedaan in het bijgeleverde Jupyter Notebook `gemeente_financien.ipynb`. De originele Excelbestanden staan in de `data` folder. De resultaten van het opschonen staan in de `data/clean` folder, deze worden in Power BI gebruikt. De tabel over de bevolking `gemeente_bevolking.xlsx` heb ik later gedownload, deze heb ik in Power Query Editor opgeschoond. 

## Vereisten
- `data/gemeente_bevolking.xlsx` 
- `data/clean/begroting_subset.xlsx`
- `data/clean/jaarrekening_subset.xlsx`
- `data/clean/begroting20-24.xlsx`
- `data/clean/jaarrekening20-22.xlsx`

## Gegevensbronnen en datasets
Alle databestanden komen van findo.nl/jive onder de kopjes 'Gemeentelijke informatie' en 'Overige gegevens' (de bevolkingsdata). Op deze website kan je zelf samenstellen welke informatie je in je tabel wil hebben. Het is niet mogelijk om te linken naar mijn precieze samenstelling, maar de financiële gegevens komen uit de informatie over 'Baten en lasten' en 'Financiële kengetallen' onder 'Gemeentelijke informatie'. De begrotingen en jaarrekeningen zijn verdeeld per taakveld. 

Findo - Data Financiën Decentrale overheden. https://findo.nl/jive?cat_open=begroting

## Navigatiegids
De 3 buttons onderaan het dashboard verwijzen naar bookmarks die de weergave van de Nederlandse kaart en de card-visual daaronder veranderen. Door op de buttons te klikken kan je op basis van het jaartal filteren welke gegevens over de gemeentelijke baten, bevolking en de afwijking van het begroot en reëel saldo van Nijkerk worden weergeven. 

## Dashboardfuncties
De kaart vergelijkt de gemeentelijke baten per inwoner van een aantal Nederlandse gemeenten. Met behulp van een filter op de bevolkingsgegevens worden alleen de gemeenten weergeven met ongeveer hetzelfde aantal inwoners als Nijkerk. Daarnaast worden in de grafieken wat financiële kengetallen van Nijkerk vergeleken met het gemiddelde voor Nederlandse gemeenten. Op de grafiek met de solvabiliteitswaarden worden ook signaleringslijnen geplot die aangeven bij welk percentage de financiële gezondheid goed of slecht is. 

De staafdiagram kijkt naar de afwijking van de baten uit de begrotings- en jaarrekeningtabellen van Nijkerk, en vergelijkt dit met het Nederlands gemiddelde. De card-visual onderaan de pagina is berekend met behulp van een DAX formule. Deze formule haalt per jaar de waarden van het saldo uit beide tabellen, en berekent het verschil. 
