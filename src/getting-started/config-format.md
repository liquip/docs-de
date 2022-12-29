# Das Konfigurations Format
Liquip benutzt eine modifizierte Version von [JSON](https://de.wikipedia.org/wiki/JavaScript_Object_Notation#Datenstruktur_und_Formatdefinition).
Wenn du nicht weißt, was JSON ist, kannst du dir den Wikipedia Artikel dazu anschauen.

Wichtig ist vor allem [dieser](https://de.wikipedia.org/wiki/JavaScript_Object_Notation#Datenstruktur_und_Formatdefinition) Unterpunkt.

## Unterschiede
Liquip lässt folgende Dinge zu:
- Tags ohne Anführungszeichen
- Kommentare
- Einzelne Anführungszeichen

Das sieht ungefähr so aus:
```JSON-Format
{
  // some comment
  name: 'value',
  'otherName': "otherValue"
}
```