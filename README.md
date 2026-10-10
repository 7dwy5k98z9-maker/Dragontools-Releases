# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## DragonTools 9.9.0 – 10.10.2026

### Funktionen

Der aktuelle Stand enthält die Hintergrundverarbeitung im Renamer und die Prüfung von Staffeln und Serien anhand der gewählten Metadatenquelle. Medienverarbeitung, Untertitelverwaltung, Warteschlange und Journal-Wiederherstellung sind enthalten. Hilfe und Changelog beschreiben die Funktionen nach technischen Themen. Einzelheiten stehen in `RELEASE_NOTES_v9.9.0.md`.

### Prüfung

Die vollständige Standardtestsuite bestand mit 5286 erfolgreichen Fällen, 18 übersprungenen Fällen und 24 nicht ausgewählten DV/HDR-Integrationstests. Datenschutzprüfung, Quellvalidierung, 18 App-Bundle-Prüfungen und der Starttest der neuen EXE bestanden.

## Windows-Paket

### Lokale Artefakte

- Vollständiges Paket: `artifacts/DragonToolsV9.9.0-win64.zip`
- Paket-Prüfsumme: `artifacts/DragonToolsV9.9.0-win64.zip.sha256`
- Anwendung: `artifacts/DragonToolsV9.9.0.exe` mit `artifacts/Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.0.exe.sha256`
- Paketgröße: 220484916 Bytes, 456 Dateien
- ZIP-SHA-256: `b978f18896da41f500752642591c6904ebef1dd4e7c8b5c170c556a5bf0f7308`
- EXE-SHA-256: `3377c704ed62f96a942892a5cff933ea33ab86cabd42a643f7065dd5d1a1a8b2`

### Installation und Download

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Das Paket enthält die notwendigen Python-/Qt-Laufzeitdateien und das öffentliche Handbuch. Externe Medienwerkzeuge werden anhand von `TOOLS_INSTALLIEREN.txt` separat eingerichtet.

Die geprüften ZIP- und SHA-256-Dateien werden im bestehenden [GitHub-Release v9.9.0](https://github.com/7dwy5k98z9-maker/Dragontools-Releases/releases/tag/v9.9.0) veröffentlicht. Entsprechend `.gitignore` bleiben die großen Binärdateien lokal unter `artifacts`; dieses Repository verwaltet die Release-Dokumentation.

Die Anwendungsversion bleibt 9.9.0. Der aktuelle öffentliche Quellcode steht in `Dragontools-Public`.

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
