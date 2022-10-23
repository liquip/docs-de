# Config Beispiel

In diesen Artikel wir Ihnen per Beispiel praktisch erklärt, ein Item zu erstellen.
Die minimalste Config ist folgende
```config
id: "liquip:test_item"
name: "Item Name"
material: "minecraft:grass_block"
```
Wie Sie sehen, erstellen Sie Items, durch das Ausfüllen mehrerer Tags. Dabei ist es wichtig zu beachten, dass die Tags
`id:`,`name:` und `material:` nicht optional sind. Das heißt das diese Tags in jeder Config existieren müssen.


Jedoch gibt es noch weitere optionale Tags, durch die Sie Ihre Config erweitern können: 
* `recipes:`
* `lore:`
* `features:`
* `enchantments:`
* `modifiers:`
* `custommodeldata:`

