# Fortgeschrittene Config-Tags

Unser Plugin ermöglicht nicht nur 3 Tags wie in [Basic Config](basic_config.md) gezeigt, sondern auch viele weitere.
Darunter sind folgende Tags:

* `lore:`
* `recipes:`
* `features:`
* `enchantments:`
* `modifiers:`
* `custommodeldata:`

Diese Tags sind nicht zwangsweise notwendig, sondern nur optional!

Außerdem gibt es noch die Möglichkeit farbige Texte zu erstellen, siehe [Farbige Namen](colorful_names.md).

## Lore-Tag
Bei diesem Tag legen Sie die Beschreibung des Items fest. Dies kann z.B. so aussehen:

```lore_tag
lore: [
  "Test Item"
  "Dies ist eine neue Zeile"
]
```

## Recipes-Tag
Beim Recipes Tag legen Sie das Crafting-Rezept für Ihr neues Item fest. Dieses Rezept ist jedoch nur im Liquip-Craftingtable
verfügbar. Dieser ist folgend aufgebaut: 

```recipes_tag
recipes: [
    {
    shape: ["xxx", " y ", " y "]
    placeholders: [
        {key: "y", type: "minecraft:stick"}
        {key: "x", type: "minecraft:diamond"}
    ]
    }
]
```

Unter ``shape:`` legt man mit Placeholdern (selbst ausgesuchte Buchstaben) das Recipe an sich fest. Diese Buchstaben
stehen für die bei ``placeholders:`` festgelegten Materialien fest. Diese können auch Liquip Items sein. In diesem
Beispiel verwenden wir das Crafting-Rezept für eine gewöhnliche Diamant-Spitzhacke. 

Die durch ein Kommatar getrennten ``Strings`` bei ``shape:`` stehen jeweils für eine Zeile im Crafting-Table.


## Features-Tag
Dieser Tag wird verwendet, um spezielle, nur per Plugin machbare Funktionen möglich zu machen. Features müssen Sie
selber im ``example-plugin`` pogrammieren und dann als Tag spezifischen Items zuweisen. 

Das zuweisen in der Config würde so aussehen:
```features_tag
features: [
  "minecraft:unbreakable"
  "liquip:test_feature"
]
```

Es gibt vorprogrammierte Features für unsere Items, wie z. B. der ``Staff of Power``, welche Sie selbstverständlich
auch zu Ihren Items hinzufügen können.

Eine Liste aller von uns pogrammierten Features finden sie [hier]().

## Enchantments-Tag