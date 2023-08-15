

## Solution

Solution Datei erstellen
```terminal
dotnet new sln
```

Projekte aus der Solution auflisten
```terminal
dotnet sln list
```

Solution Datei mit festgelegeten Name erstellen
```terminal
dotnet new sln --name <solutionname>
```

Projekt zur einer solution hinzufügen
```terminal
dotnet sln add <path-to-project.csproj>
```

Projekt zur einer festgelegten Solution Datei hinzufügen
```terminal
dotnet sln <path-to-solution.sln> add <path-to-project.csproj>
```

Projekt aus einer Solution entfernen
```terminal
dotnet sln remove <path-to-project.csprojcsproj>
```

### Projekte hinzufügen

Projekttemplates anzeigen
```terminal
dotnet new list
```

Projekt hinzufügen
```terminal
dotnet new <projekttemplate>
``` 

### Packetverwaltung

Nuget Packet hinzufügen
Hierfür muss man sich in den Ordner des Ausgewählten Projektes befinden.
```terminal
dotnet add package <name>
```

