# Cheat Sheet für die Linux Kommandozeile

##Dateien

Dateien Anzeigen
```bash
ls
```

Dateien Anzeigen mit versteckten Dateien
```bash
ls -a
```

Dateien Anzeigen für Menschen lesbar
```bash
ls -h
```

Dateien Anzeigen ausgabe als liste
```bash
ls -l
```

Dateien suchen auf basis des Index
```bash
find
```

Dateien anlegen
```bash
touch
```

Verzeichnis erstellen
```bash
mkdir
```

Dateien löschen
```bash
rm
```

rekursiv löschen
```bash
rm -r
```

force löschen
```bash
rm -f
```

Verzeichnis löschen
```bash
rmdir
```

Kopieren einer Datei, Konvertierung und Formatierung
z. B Img to UsbBootStick
```bash
dd
```

## Laufwerke, Partitionen & Co.

Alle Festplatten
```bash
lshw
lshw -class disk -short
```

Alle Blockgeräte
```bash
lsblk
```
Partitionsnamen, UUID und Label
```bash
blkid
```

Verfügbarer Festplattenspeicher
```bash
df
```

Verfügbarer Festplattenspeicher mit besserer Größenangabe
```bash
df -h
```

Benutzter Festplattenspeicher
```bash
du
du -sh
```
