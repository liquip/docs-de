# Installation
Um das Plugin zu installieren, müssen Sie es derzeit selbst erstellen. In der folgenden Anleitung wird Ihnen dies Schritt für Schritt beigebracht.

## Voraussetzungen
Um das Plugin zu bauen, benötigen Sie Folgendes:
* Java 17 oder höher
* Git

## Java installieren
Um Java zu installieren, können Sie zu [Adoptium](https://adoptium.net) gehen. Sie bieten vorgefertigte Java-Binaries und sogar Installer für Java.

## Git installieren
Um Git zu installieren, können Sie zu <https://git-scm.com/downloads> gehen und Git von dort installieren.

## Konfiguration
Um das Projekt einzurichten, müssen Sie zuerst das Repository klonen. Erstellen Sie dazu irgendwo ein Verzeichnis und öffnen Sie dort Ihr Terminal und führen Sie den folgenden Befehl aus:
```sh
git clone https://github.com/liquip/liquip-plugin.git .
```
Dadurch wird das Repository in das aktuelle Verzeichnis geklont. Beachten Sie, dass das Verzeichnis dazu leer sein muss.

## JAR-Datei bekommen 
Um das Plugin (.jar-Datei) jetzt zu erstellen, führen Sie den folgenden Befehl in dem Verzeichnis aus, in das Sie geklont haben:

Für Linux/macOS:
```sh
./gradlew build
```

Für Windows:
```bat
.\gradlew.bat build
```

Dies sollte Gradle starten und das Plugin erstellen. Das Plugin ist in drei Submodule unterteilt, nämlich 'core', 'example-plugin' und 'gui'. Das Kernmodul ist das Liquip-Plugin. Das Beispiel-Plugin enthält einige experimentelle Features. Das GUI-Modul enthält den Code für die Inventory-GUIs. Alle drei Module werden gebaut, aber Sie interessieren sich höchstwahrscheinlich nur für das Kernmodul. Die Ausgabe befindet sich im Verzeichnis `core/build/libs`. Sie möchten die JAR-Datei ohne '-dev' oder '-all' darin nehmen und sie in Ihr Plugins-Verzeichnis legen.