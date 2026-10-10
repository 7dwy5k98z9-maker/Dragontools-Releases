# Veröffentlichung von DragonTools 9.9.0

## Quellstand

### Abgleich und Prüfungen

Privaten und öffentlichen Quellstand abgleichen. Hilfe und Changelog aktuell halten. Datenschutzprüfung, Standardtests und Release-Validierung ausführen.

## Windows-Paket

### Build und Laufzeit

Die EXE aus dem öffentlichen Quellstand ohne externe Medienwerkzeuge bauen. App-Bundle, kompilierte Anwendungsmodule und den Start der tatsächlichen EXE prüfen.

### Artefakte

Die EXE mit vollständigem Daten-Ordner unter artifacts ablegen. Den Anwendungsordner als ZIP verpacken, dessen Inhalt und CRC prüfen sowie SHA-256-Dateien für EXE und ZIP erstellen.

## Veröffentlichung

### Repositories und GitHub-Release

Quellstand und Release-Dokumentation committen und pushen. Das bestehende GitHub-Release v9.9.0 mit dem geprüften ZIP und seiner Prüfsumme aktualisieren. Die zusätzlichen lokalen Dateien bleiben unter artifacts erhalten.
