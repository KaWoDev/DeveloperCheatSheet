# Sheet Cheat - Git Versionsverwaltung

Internetseite
Offiziele Internetseite (https://git-scm.com/)

## Hilfe und Info

Git Version anzeigen
```terminal
git --version
```
Hilfe anzeigen im Terminal/ terminal ...
```terminal
git help
```
Hilfe anzeigen **z.b für Branches** im Browser anzeigen (lokal)
```terminal
git help <branch>
```

## Einrichtung

Globalen Benutzernamen setzen
```terminal
git config --global user.name <name>
```

Globalen Benutzernamen setzen
```terminal
git config --global user.email <email>
```

## Repository erstellen oder Klonen

Repository Anlegen
``git init``

Repository aus Origin auf den Pc Klonen
```terminal
git clone git://...
git clone ssh://...
```

Status anzeigen
```terminal
git status
```

## Stages und Commits erstellen

Änderungen in den Stage verschieben
```terminal
git add ...
```
Änderungen ausgewählter Dateien in den Stage verschieben
```terminal
git add <datei1> <datei2> 
```

Alle änderungen in den Stage verschieben
```terminal
git add -A
git add --all
```

Änderungen **ab den aktuellen Verzeichnis** in den Stage verschieben
```terminal
git add .
```

Commit erstellen - Editor zur Eingabe einer Nachricht wird geöffnet
```terminal
git commit
```

Commit erstellen mit Nachricht erstellen
```terminal
git commit -m <Nachricht>
git commit --message <Nachricht>
```

Letzten Commit überschreiben
ACHTUNG nur nutzen, wenn noch nicht gepusht wurde!!
```terminal
git commit --amend
```

Letzten Commit überschreiben und Message übernehmen
ACHTUNG nur nutzen, wenn noch nicht gepusht wurde!!
```terminal
git commit --amend --no-edit
```

## Logeinträge

Log anzeigen
```terminal
git log
```

letzte n logs anzeigen
```terminal
git log -n
```

Logeintrag einzeilig
```terminal
git log --oneline
```

Logeinträge Farbig
```terminal
git log --pretty
```

Logeinträge mit graphen
```terminal
git log --graph
```

Logeinträge mit einem suchbegriff im Kommentar
```terminal
git log --grep <suchbegriff>
```

Referenzlog anzeigen
Beinhaltet auch gelöschte oder überschriebene einträge, sofern diese noch im Repo vorhanden sind
gleiche Parameter wie bei log möglich
```terminal
git reflog
```

## Referenzen

HEAD Letzter Commit
HEAD^ Vorletzter Commit
HEAD~n n-ter letzter Commit

## Branches

Branch anlegen
```terminal
git branch <name>
```

Branch anlegen und gleichzeitig in den neuen Branch wechseln
```terminal
git switch -c <name>
git checkout -b <name>
```

Branch wechseln
```terminal
git switch <name>
    git checkout <name>
```

Branch löschen
```terminal
git branch -D <name>
```

## Änderungen verwerfen/ rückgängig machen

Alle änderungen verwerfen, die im Stage bereich sind
```terminal
git reset --hard
```

```terminal
git restore
```

## Aufräumarbeiten

Nicht von Git verwaltete Dateien löschen
```terminal
git clean 
``

Nicht von Git verwaltete rekursiv Dateien löschen
```terminal
git clean -d
``

Nicht von Git verwaltete inkl. Dateien aus .gitignore Dateien löschen
```terminal
git clean -x
```