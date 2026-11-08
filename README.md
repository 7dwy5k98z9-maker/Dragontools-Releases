# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## DragonTools 9.9.3 – 08.11.2026

Version 9.9.3 verbessert die Suche nach verkürzten Serientiteln und Umlaut-Schreibweisen. Die Filmbewertung erhält keinen pauschalen Bonus mehr durch ein passendes Jahr. Bei der Untertitel-Extraktion können mehrere Sprachen gewählt werden; die Wahl des Film-Zielordners wurde präzisiert. Der Windows-Energieschutz verwendet Anforderungen für laufende Aufträge.

Einzelheiten stehen in [RELEASE_NOTES_v9.9.3.md](RELEASE_NOTES_v9.9.3.md).

## Windows-Paket

- Vollständiges Paket: `artifacts/DragonToolsV9.9.3-win64.zip`
- ZIP-Prüfsumme: `artifacts/DragonToolsV9.9.3-win64.zip.sha256`
- Anwendung: `artifacts/DragonToolsV9.9.3/DragonToolsV9.9.3.exe` mit zugehörigem `Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.3/DragonToolsV9.9.3.exe.sha256`, zusätzlich unter `artifacts/`
- Paketgröße: 208105927 Bytes, 455 Dateien
- ZIP-SHA-256: `7826a36837b4346928f73c84e1ba0a841388d77b8193e5580d390d3c397b370c`
- EXE-SHA-256: `f1a4b4e09cb7ba435673199b0300ee1c901af0646ff597f6b419bcaa655e6308`

Das vollständige ZIP entpacken und EXE und Ordner `Daten` zusammen belassen. Python-/Qt-Laufzeitdateien und das eigenständige Handbuch mit 408 Seiten sind enthalten. Externe Medienwerkzeuge werden anhand von `TOOLS_INSTALLIEREN.txt` separat eingerichtet.

ZIP und Prüfsummen stehen im [GitHub-Release v9.9.3](https://github.com/7dwy5k98z9-maker/Dragontools-Releases/releases/tag/v9.9.3). Große Binärdateien bleiben gemäß `.gitignore` außerhalb der Git-Historie. Ältere Versionen und lokale Artefakte bleiben erhalten.

## Prüfungen und Quellcode

Die öffentliche Standardtestsuite bestand: `5741 passed, 20 skipped, 24 deselected in 437.10s (0:07:17)`. Auch die private Standardtestsuite und die zusätzlichen nativen Windows-Fenstertests bestanden. Datenschutzprüfung, statische Prüfung, Quellvalidierung, Paketvalidierung und EXE-Starttest waren erfolgreich. Alle 934 enthaltenen Anwendungsmodule wurden gegen den Quellstand geprüft; ZIP-CRC und SHA-256 sind verifiziert.

Öffentlicher Quellstand: [533c263](https://github.com/7dwy5k98z9-maker/Dragontools-Public/commit/533c263e8a4440a62810fcf451834ea34464ad13).

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
