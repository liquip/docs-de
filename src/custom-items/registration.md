# Registration
Bevor du endlich dein erstes Item erstellen kannst, musst du erstmal wissen, wie du deine eigenen Items registrierst.

### Was bedeutet eigentlich Registrieren?
Bei Liquip muss man seine Items nochmal in einer Hauptkonfigdatei auflisten. Man gibt immer den Pfad und den Namen
deines neuen Items in solch einer Konfigdatei an, damit das Plugin später weiß, wo sich deine Konfigurationsdateien
für deine Items befinden. 

Dies ist zwingend Nötig, wenn du deine Items später in Minecraft sehen möchtest.

## Ordnerstruktur
Aktuell müsste die Ordnerstruktur in `plugins/liquip` so aussehen:
```file_structure_first
└── config.json
```
Jetzt musst du nor noch einen Überbegriff erstellen, unter dem du deine Items auflistest. Am besten nennst du ihn
ungefähr so: `items`

Die Konfigurationsdatei würde dann so aussehen:
```file_structure_medium
.
├── config.json
└── items
   ├── bedrock_pickaxe.json
   └── bedrock_sword.json
```

Du kannst auch weitere Unterordner für jede namespace erstellen.

```file_structure_max
.
├── config.json
└── items
    └── mynewitems
        ├── bedrock_pickaxe.json
        └── bedrock_sword.json
```

## Registration
Um die Items nun zu registrieren, musst du in die `config.json` folgenden Code eingeben:
```config.json
{
  "items": [
    "<Pfad zu deinem Item>/<Dateiname (.json)>"
  ]
}
```

Wenn du deine Items später erstellt hast, müsste deine Konfigurationsdatei dann ungefähr so aussehen:
```finished config.json
{
  "items": [
    "items/mynewitems/bedrock_pickaxe.json",
    "items/mynewitems/bedrock_sword.json"
  ]
}
```