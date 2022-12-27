# Installation
Um Liquip zu installieren, müssen Sie die letzte Version von der [Github Releases Seite](https://github.com/liquip/liquip-plugin/releases)
herunterladen. 

Wenn Sie die [JAR-Datei](https://de.wikipedia.org/wiki/Java_Archive) heruntergeladen haben, sollten Sie diese in das
`plugin` Verzeichnis Ihres Servers verschieben. Wenn Sie noch keinen Server aufgesetzt haben finden Sie auf dieser Seite
eine Anleitung dafür.

## Voraussetzungen
Um Liquip benutzen zu können brauchen Sie folgendes:
- Java 17 oder neuer
- Paper 1.19 Server (andere Versionen sind nicht getestet)

## Installation von Java
Falls Sie kein Java installiert haben können Sie zu [Adoptium](https://adoptium.net/de/) gehen und sich dort die Java Binarys und sogar fertige Installer
herunterladen.

Um zu testen, ob Sie Java erfolgreich installiert haben, müssen Sie Ihre Konsole öffnen und dort den Befehl `java --version` eingeben.
Sie werden danach eine Antwort wie `openjdk 17.0.1 2021-10-19` erhalten. Wichtig ist die erste Zahl nach `openjdk` 17 oder höher ist.

## Installation von Paper und Aufsetzen des Minecraft-Servers
Um Ihren persönlichen Minecraft Server zu erstellen, müssen Sie sich erstmal die neuste Paper-Version von deren [Website](https://papermc.io/downloads)
herunterladen und die heruntergeladene JAR-Datei zu Ihrem gewünschten Verzeichnis verschieben. 

Um danach den Server zu starten, müssen Sie Ihr Terminal in dem Verzeichnis öffnen und folgenden Befehl ausführen:
`java -Xms2G -Xmx2G -jar <Dateiname der JAR-Datei + .jar> --nogui` also z. B. `java -Xms2G -Xmx2G -jar paper-1.19.3-362.jar --nogui`.

Beim ersten Start der Datei wird höchstwahrscheinlich ein Error auftreten. Die Error-Nachricht müsste ungefähr so aussehen:
`Failed to load eula.txt`. Dies ist völlig normal und heißt einfach, dass Sie dem [Endbenutzer-Lizensvertrag](https://de.wikipedia.org/wiki/Endbenutzer-Lizenzvertrag) zustimmen müssen.

Dafür öffnen Sie die neu erstellte Datei `eula.txt`. In dieser müsste ungefähr das stehen:
```eula
#By changing the setting below to TRUE you are indicating your agreement to our EULA (https://aka.ms/MinecraftEULA).
#Tue Dec 27 18:00:00 CET 2022
eula=false
```
Schreiben Sie das letzte Wort in dieser Datei von `false` zu `true`.

Wenn Sie das erledigt haben, können Sie den Server über den gleichen, schon ausgeführten Befehl starten.

Jetzt müsste sich auch ein `plugin` Ordner erstellen, in den Sie die Liquip-Datei hineinkopieren. (s. o.)

Um das Plugin zu laden, müssen Sie den Server neu starten. Das geht mit dem Befehl `stop` und nach dem erfolgreichen
Stoppen des Servers geben Sie einfach wieder den vorher verwendeteten Start-Befehl ein.