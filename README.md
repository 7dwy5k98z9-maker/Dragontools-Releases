# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## DragonTools 9.9.2 – 23.10.2026

Version 9.9.2 enthält konfigurierbare Standarduntertitel, verbesserte Audio-Spracherkennung und Serienzuordnung, Mediathekimport mit Fortschrittsanzeige sowie Korrekturen an Verschieben, Warteschlange, Laufzeitprüfung und Windows-Neustartschutz. Einzelheiten stehen in [RELEASE_NOTES_v9.9.2.md](RELEASE_NOTES_v9.9.2.md).

## Windows-Paket

- Vollständiges Paket: `artifacts/DragonToolsV9.9.2-win64.zip`
- Paket-Prüfsumme: `artifacts/DragonToolsV9.9.2-win64.zip.sha256`
- Anwendung: `artifacts/DragonToolsV9.9.2/DragonToolsV9.9.2.exe` mit zugehörigem `Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.2/DragonToolsV9.9.2.exe.sha256`, zusätzlich unter `artifacts/`
- Paketgröße: 214315722 Bytes, 455 Dateien
- ZIP-SHA-256: `259bc868c940751713603071cf6e3de51f83b27da523351989b2e6e52a5b7766`
- EXE-SHA-256: `55f658cc341d2e5f80e5d8f1e9c9ec069044a6f717a2fa069b1c53b612447ea1`

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Das Paket enthält die benötigten Python-/Qt-Laufzeitdateien und das öffentliche Handbuch mit 408 Seiten. Externe Medienwerkzeuge werden separat anhand von `TOOLS_INSTALLIEREN.txt` eingerichtet.

ZIP und Prüfsummen stehen im [GitHub-Release v9.9.2](https://github.com/7dwy5k98z9-maker/Dragontools-Releases/releases/tag/v9.9.2). Entsprechend `.gitignore` bleiben die großen Binärdateien lokal unter `artifacts`; dieses Repository verwaltet die Release-Dokumentation. Ältere Veröffentlichungen bleiben verfügbar.

## Prüfungen und Quellcode

Die vollständige öffentliche Standardtestsuite bestand: `5658 passed, 20 skipped, 24 deselected in 466.06s (0:07:46)`. Die zwei nativen Windows-Neustartschutztests bestanden zusätzlich. Datenschutzprüfung, statische Prüfung, Quellvalidierung, App-Validierung und EXE-Starttest bestanden. Alle 930 enthaltenen Anwendungsmodule wurden gegen den aktuellen Quellstand geprüft. ZIP-Inhalt, CRC und SHA-256 sind verifiziert.

Der öffentliche Quellcode steht in [Dragontools-Public](https://github.com/7dwy5k98z9-maker/Dragontools-Public).

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
