# H1 Suomen kunnat ja kuntien rajat excelissä sekä json-tiedostossa.
Postinumerot ja niiden rajat json-tiedostossa.

Jos tarvetta niin lataa itsellesi :)

Tässä muutama esimerkki kunnanrajoista:
1. https://s2koulut.vercel.app/
2. https://vaestonkehitys2021.vercel.app/
3. https://rikokset.vercel.app/

postinumerot.json:
[
 {
  "postinumeroalue": "00100",
  "koordinaatit": [[24.93330585,60.16509986],[24.94347937,60.16640484],[24.95129163,60.1679147],[24.94187067,60.17730052],[24.93504055,60.17895103],[24.912563,60.17580059],[24.91282158,60.17029852],[24.93330585,60.16509986]]
 },
 {
  "postinumeroalue": "00120",
  "koordinaatit": [[24.92854196,60.1610119],[24.94649431,60.16101796],[24.94347937,60.16640484],[24.93330585,60.16509986],[24.92854196,60.1610119]]
 },
 ...
]

postinumerot_geo.json:
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": { "kunta": "Helsinki", "postinumeroalue": "00100" },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [24.93330585, 60.16509986],
            [24.94347937, 60.16640484],
            [24.95129163, 60.1679147],
            [24.94187067, 60.17730052],
            [24.93504055, 60.17895103],
            [24.912563, 60.17580059],
            [24.91282158, 60.17029852],
            [24.93330585, 60.16509986]
          ]
        ]
      }
    },
    {
      "type": "Feature",
      "properties": { "kunta": "Helsinki", "postinumeroalue": "00120" },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [24.92854196, 60.1610119],
            [24.94649431, 60.16101796],
            [24.94347937, 60.16640484],
            [24.93330585, 60.16509986],
            [24.92854196, 60.1610119]
          ]
        ]
      }
    },
	...
	]
}

