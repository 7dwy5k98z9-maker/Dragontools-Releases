# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## DragonTools 9.9.2 – aktualisiert am 24.10.2026

Der aktuelle Build berücksichtigt konfigurierte Titel-Aliasse auch bei der Prüfung von TheTVDB-Detaildaten. So werden passende Treffer mit abweichendem deutschen oder englischen Titel nicht vorzeitig verworfen. Die Prüfung des Serienjahrs bleibt erhalten. Zusätzliche alternative Staffelzählungen wurden nicht eingeführt.

Die weiteren Änderungen der Version stehen in [RELEASE_NOTES_v9.9.2.md](RELEASE_NOTES_v9.9.2.md).

## Windows-Paket

- Vollständiges Paket: `artifacts/DragonToolsV9.9.2-win64.zip`
- Paket-Prüfsumme: `artifacts/DragonToolsV9.9.2-win64.zip.sha256`
- Anwendung: `artifacts/DragonToolsV9.9.2/DragonToolsV9.9.2.exe` mit zugehörigem `Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.2/DragonToolsV9.9.2.exe.sha256`, zusätzlich unter `artifacts/`
- Paketgröße: 214317033 Bytes, 455 Dateien
- ZIP-SHA-256: `7f0c3f161bc80ddae949bcd3ea71694bde9e7b2b5dc508941c47116bc40de58f`
- EXE-SHA-256: `d364b95dbdc4bc04bb2d986da4d13a76fd46cc2dd205d41f561769f670a9554c`

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Python-/Qt-Laufzeitdateien und das eigenständige Handbuch sind enthalten. Externe Medienwerkzeuge werden separat anhand von `TOOLS_INSTALLIEREN.txt` installiert.

ZIP und Prüfsummen stehen im [GitHub-Release v9.9.2](https://github.com/7dwy5k98z9-maker/Dragontools-Releases/releases/tag/v9.9.2). Große Binärdateien bleiben gemäß `.gitignore` außerhalb der Git-Historie. Der vorherige lokale Build ist unter `artifacts/previous-20261024/` gesichert.

## Prüfungen und Quellcode

Die vollständige öffentliche Standardtestsuite bestand: `5665 passed, 20 skipped, 24 deselected in 306.74s (0:05:06)`. 160 gezielte Tests im privaten Projekt bestanden ebenfalls. Statische Prüfung, Datenschutzprüfung, Quellvalidierung, Paketvalidierung und EXE-Starttest bestanden. Alle 930 enthaltenen Anwendungsmodule wurden gegen den aktuellen Quellstand geprüft; ZIP-CRC und SHA-256 sind verifiziert.

Öffentlicher Quellstand: [d8a7189](https://github.com/7dwy5k98z9-maker/Dragontools-Public/commit/d8a71895f0bef86afc2d54f2007339034c16791e).

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
