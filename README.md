# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## DragonTools 9.9.1 – 13.10.2026

### Medienverarbeitung und Dateiverwaltung

Der aktuelle Stand korrigiert die Laufzeit beim Einbrennen von PGS-Untertiteln und setzt passende Untertitel bei anderssprachigem Audio automatisch als Standard. Der MP4-Remux verwendet die vorhandene Analyse; die Videoliste zeigt die geplante Pipeline. Video- und Audiodauer werden getrennt geprüft, erfolgreiche Reparaturen hinterlassen keine unveränderten Zwischenkopien desselben Auftrags. Bestätigte Renamer-Zuordnungen werden im Preflight wiederverwendet; der Verschiebeablauf vermeidet zusätzliche vollständige Dateizugriffe. Staffel- und Serienprüfung sowie Journal-Wiederherstellung sind enthalten. Einzelheiten stehen in [RELEASE_NOTES_v9.9.1.md](RELEASE_NOTES_v9.9.1.md).

### Dokumentation und Prüfungen

Hilfe, Handbuch und Changelog sind auf Version 9.9.1 abgestimmt. Das eigenständige Anwender-, Referenz- und Entwicklerhandbuch wird aus der Word-Quelle gepflegt und behält seine 35 Hauptkapitel auf 408 Seiten. Die Standardtestsuite bestand mit 5401 erfolgreichen Fällen, 13 übersprungenen Fällen und 24 nicht ausgewählten DV/HDR-Integrationstests. Die Veröffentlichung umfasst die statische Codeprüfung, die öffentliche Datenschutzprüfung, die Quellvalidierung und den Starttest der tatsächlichen EXE. Die 18 App-Prüfpunkte ergeben keine Fehler; externe Medienwerkzeuge werden separat installiert.

## Windows-Paket

### Lokale Artefakte

- Vollständiges Paket: `artifacts/DragonToolsV9.9.1-win64.zip`
- Paket-Prüfsumme: `artifacts/DragonToolsV9.9.1-win64.zip.sha256`
- Anwendung: `artifacts/DragonToolsV9.9.1/DragonToolsV9.9.1.exe` mit zugehörigem `Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.1/DragonToolsV9.9.1.exe.sha256`, zusätzlich im Wurzelordner `artifacts/`
- Paketgröße: 205927448 Bytes, 409 Dateien
- ZIP-SHA-256: `348725aa46b838f7a3aca8aa915424d962caa07bb2a8afbf852aab167459b07a`
- EXE-SHA-256: `cc746f9019716a0e171eb27a39cee0cee55257b5bc8d0a2771b0d37d63574879`

### Installation und Download

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Das Paket enthält die benötigten Python-/Qt-Laufzeitdateien und das öffentliche Handbuch. Externe Medienwerkzeuge werden anhand von `TOOLS_INSTALLIEREN.txt` separat eingerichtet.

ZIP und Prüfsummen stehen im [GitHub-Release v9.9.1](https://github.com/7dwy5k98z9-maker/Dragontools-Releases/releases/tag/v9.9.1). Entsprechend `.gitignore` bleiben die großen Binärdateien lokal unter `artifacts`; dieses Repository verwaltet die Release-Dokumentation. Ältere Veröffentlichungen bleiben verfügbar.

### Quellcode

Die Anwendungsversion ist 9.9.1. Der öffentliche Quellcode steht in [Dragontools-Public](https://github.com/7dwy5k98z9-maker/Dragontools-Public).

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
