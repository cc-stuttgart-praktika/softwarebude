# Wie du mitmachen kannst

## Abhängigkeiten installieren
Zum Installieren aller für das Entwickeln des Spiels notwendigen Abhängigkeiten gehst du wie folgt vor.

### pipenv als Paketmanager
Installiere [pipenv](https://pipenv.readthedocs.io/) zum Verwalten von Abhängigkeiten.
Auf einem Rechner mit MacOS und [Homebrew](https://brew.sh/) nutzt du folgenden Befehl:
```
brew install pipenv
```
Alternativ ist auch die Installation über [pip](https://pip.pypa.io/en/stable/) möglich:
```
pip install --user pipenv
```

### Projektabhängigkeiten
Installiere alle Abhängigkeiten für dieses Projekt.
Führe dazu folgenden Befehl im Rootverzeichnis des Projekts aus:
```
pipenv install
```
Neue Abhängigkeiten kannst du wie folgt hinzufügen:
```
pipenv install <package-name>
```
Mehr Informationen dazu findest du in der Dokumentation von pipenv zum Thema [Installieren von Paketen](https://pipenv.readthedocs.io/en/latest/install/#installing-packages-for-your-project).


### pre-commit Hooks
Wir verwenden [pre-commit](https://pre-commit.com/#intro) um vor jedem Git `commit` den Programmcode einheitlich zu formatieren.
Zum aktivieren der in `.pre-commit-config.yaml` definierten Hooks, führe bitte folgenden Befehl aus:
```
pipenv run pre-commit install
```

## Code Formatierung
Wir nutzen [Black](https://black.readthedocs.io/en/stable/#) zum automatisierten Formatieren von Python Code.
Black kannst du auch [für deine Entwicklungsumgebung einrichten](https://black.readthedocs.io/en/stable/editor_integration.html).