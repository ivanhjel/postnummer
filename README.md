# Postnummerområder i .geojson. 

Hele Norge er delt inn i postnummerområder og datasettet fra Kartverket gir deg de offisielle postnumrenes utstrekning i areal.

Datasettet er tilgjengelig her:
https://data.norge.no/data/statens-kartverk/postkretser-i-norge

# Problemet

Datasettet er kun tilgjengelig i WFS, GML eller SOSI. 

# Løsningen

1. GML ble konvertert til geojson. 
2. Unødvendige datafelter ble fjernet med CartoDB. 
3. Douglas-Peucker algoritmen ble brukt for å redusere filen fra 75mb til 5mb uten at det gikk utover kvaliteten til datasettet. 

