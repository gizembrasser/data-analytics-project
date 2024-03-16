# Het eindproject - Gemeentelijke financiën Nijkerk

Link naar Github repository: https://github.com/gizembrasser/data-analytics-project

## Beschrijving
Dit dashboard weergeeft informatie over de gemeentelijke financiën van Nijkerk vergeleken met de rest van Nederlandse gemeenten. De data is afkomstig uit de begrotingen (2020 - 2024) en jaarrekeningen (2020 - 2022) van alle gemeenten, en uit bevolkingsgegevens van deze gemeenten. Het doel van het dashboard is om de volgende businessvragen te beantwoorden: 

1. Hoe groot is het verschil tussen het saldo van de begroting/jaarrekening in Nijkerk vergeleken met de rest van de gemeenten?
2. Hoeveel verdient de gemeente Nijkerk aan baten vergeleken met andere gemeenten?
3. Bewoners in Nijkerk vinden dat er opvalled veel leegstand is; hoe vergelijkt de grondexploitatie met de rest van de gemeenten?
4. Hoe vergelijkt de solvabiliteit van de gemeente Nijkerk met de rest van de gemeenten?
5. Zijn er financiële kengetallen die alarmbellen moeten gaan rinkelen bij de gemeente Nijkerk?

## Installatie-instructies
De datatransformatie is gedaan in het bijgeleverde Jupyter Notebook `gemeente_financien.ipynb`. De originele Excelbestanden staan in de `data` folder, en de resultaten van het opschonen staan in de `data/clean` folder, deze worden in Power BI gebruikt. De tabel over de bevolking `gemeente_bevolking.xlsx` heb ik later gedownload, deze heb ik in Power Query Editor opgeschoond. 

## Vereisten
- `data/gemeente_bevolking.xlsx` 
- `data/clean/begroting_subset.xlsx`
- `data/clean/jaarrekening_subset.xlsx`
- `data/clean/begroting20-24.xlsx`
- `data/clean/jaarrekening20-22.xlsx`

