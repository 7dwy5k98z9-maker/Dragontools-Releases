# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## DragonTools 9.9.1 – 12.10.2026

### Medienverarbeitung und Untertitel

Der aktuelle Stand korrigiert die Laufzeit beim Einbrennen von PGS-Untertiteln und setzt passende Untertitel bei anderssprachigem Audio automatisch als Standard. Der MP4-Remux verwendet die vorhandene Analyse; die Videoliste zeigt die geplante Pipeline. Renamer, Staffel- und Serienprüfung sowie Journal-Wiederherstellung sind enthalten. Einzelheiten stehen in [RELEASE_NOTES_v9.9.1.md](RELEASE_NOTES_v9.9.1.md).

### Dokumentation und Prüfungen

Hilfe, Handbuch und Changelog sind auf Version 9.9.1 abgestimmt. Die Standardtestsuite bestand mit 5365 erfolgreichen Fällen, 13 übersprungenen Fällen und 24 nicht ausgewählten DV/HDR-Integrationstests. Die statische Codeprüfung, die öffentliche Datenschutzprüfung, die Quellvalidierung und der Starttest der tatsächlichen EXE bestanden. Die 18 App-Prüfpunkte ergeben keine Fehler; externe Medienwerkzeuge werden separat installiert.

## Windows-Paket

### Lokale Artefakte

- Vollständiges Paket: `artifacts/DragonToolsV9.9.1-win64.zip`
- Paket-Prüfsumme: `artifacts/DragonToolsV9.9.1-win64.zip.sha256`
- Anwendung: `artifacts/DragonToolsV9.9.1/DragonToolsV9.9.1.exe` mit zugehörigem `Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.1/DragonToolsV9.9.1.exe.sha256`, zusätzlich im Wurzelordner `artifacts/`
- Paketgröße: 198092146 Bytes, 409 Dateien
- ZIP-SHA-256: `c07d5384b0faa175fa4448f997c18e6d19c60c7baa4b8a1b0a3657f0676ff0a1`
- EXE-SHA-256: `7638eb1ff2794a68c0c3bdacb06cd0e688113d1c7329eb6fdb8410c83733894e`

### Installation und Download

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Das Paket enthält die benötigten Python-/Qt-Laufzeitdateien und das öffentliche Handbuch. Externe Medienwerkzeuge werden anhand von `TOOLS_INSTALLIEREN.txt` separat eingerichtet.

ZIP und Prüfsummen stehen im [GitHub-Release v9.9.1](https://github.com/7dwy5k98z9-maker/Dragontools-Releases/releases/tag/v9.9.1). Entsprechend `.gitignore` bleiben die großen Binärdateien lokal unter `artifacts`; dieses Repository verwaltet die Release-Dokumentation. Ältere Veröffentlichungen bleiben verfügbar.

### Quellcode

Die Anwendungsversion ist 9.9.1. Der öffentliche Quellcode steht in [Dragontools-Public](https://github.com/7dwy5k98z9-maker/Dragontools-Public).

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
