# Das Konfigurationsformat

Viele Plugins verwenden die [YAML-Konfigurationssprache] (https://en.wikipedia.org/wiki/YAML). Wir verwenden stattdessen ein anderes
Konfigurationsformat. Wir denken, dass es weniger fehleranfällig ist, da es nicht auf Einrückungen angewiesen ist. Es heißt HOCON und wir empfehlen es
die Dateierweiterung `.conf`. Um mehr darüber zu erfahren, klicken sie
[hier](https://github.com/lightbend/config/blob/4458ea947a7a2a668bb811a122455f1f05975172/HOCON.md), aber wir werden es auch tun
erklären die Grundlagen in dieser kurzen Anleitung.

## Datentypen

In HOCON gibt es folgende Datentypen:
* Object
* List
* Integer
* Floating-point number
* String/Text
* Boolean (true/false)
## Darstellung

Die Konfigurationsdatei selbst ist ein Objekt. Es enthält Schlüssel-Wert-Paare. Um einer Taste einen Wert zuzuweisen, schreiben Sie die Taste gefolgt von der Taste
durch ein Gleichheitszeichen (`=`) oder einen Doppelpunkt (`:`) gefolgt vom Wert. Das wird so aussehen:
```hocon
some_value: 42
```
oder
```hocon
some_other_value: 13
```
### Einfache Typen

Ganze Zahlen werden einfach ausgeschrieben (z. B. `123`).

Floats werden mit einem Punkt als Trennzeichen geschrieben (z. B. `4.5`).

Strings werden in doppelte Anführungszeichen geschrieben (z. B. `"Hello, world!"`).

Boolesche Werte werden als wahr oder falsch geschrieben (z. B. „true“).

### Objekte

Objekte werden als Schlüssel-Wert-Paare geschrieben, die von geschweiften Klammern (`{}`) umgeben und durch Kommas oder Zeilenumbrüche getrennt sind.

Das Zuweisen eines Objekts zu einer Taste kann wie folgt aussehen:

```hocon
some_object: {some_string = "Hey", some_number = 456}
```

oder:

```hocon
some_other_object: {
  some_other_string: "Hey"
  some_other_number: 456
}
```