# DragonTools Releases

Öffentliche Veröffentlichungsinformationen unter dem Entwicklernamen **Dragon Developer**.

## Aktueller Stand: DragonTools 9.9.0 – 08.10.2026

Der aktuelle Windows-Build enthält die Korrekturen für Timestamp-Reparatur, erneutes Hinzufügen entfernter Dateien, Journal-Wiederherstellung beim Start, Schriftanhänge beim Untertitel-Einfügen, WebVTT-Zuordnung und Strip-only-Audiometadaten. Alle bisherigen 29 Review-Schritte bleiben enthalten. Einzelheiten stehen in `RELEASE_NOTES_v9.9.0.md`.

Die vollständige Standardtestsuite umfasst 5234 bestandene Fälle, 18 übersprungene Fälle und 24 abgewählte DV/HDR-Integrationstests. Datenschutz-, Syntax-, Architektur-, Paket- und EXE-Startprüfung bestanden.

## Lokale Artefakte

- Anwendung: `artifacts/DragonToolsV9.9.0.exe` mit `artifacts/Daten/`
- EXE-Prüfsumme: `artifacts/DragonToolsV9.9.0.exe.sha256`
- Vollständiges Paket: `artifacts/DragonToolsV9.9.0-win64.zip`
- Paket-Prüfsumme: `artifacts/DragonToolsV9.9.0-win64.zip.sha256`
- Paketgröße: 220660941 Bytes, 455 Dateien
- ZIP-SHA-256: `84a4e8559b9f02452fce9632f31231e96ed1509e976857679d34e69b0b115c0b`
- EXE-SHA-256: `4fdd427557b1d121fd5e9c92444e215c3b56dea4c183cbd600e0001ca8fc53de`

ZIP und Prüfsummen wurden nach der Erstellung erneut kontrolliert. Das Paket enthält die notwendigen Python-/Qt-Laufzeitdateien und das öffentliche Handbuch. Externe Medienwerkzeuge werden anhand von `TOOLS_INSTALLIEREN.txt` separat eingerichtet.

## Repository und Installation

Der Git-Push aktualisiert diese Release-Dokumentation. Die Artefakte bleiben zusätzlich entsprechend `.gitignore` lokal unter `artifacts`. Das bestehende GitHub Release `v9.9.0` wird mit dem geprüften vollständigen ZIP und seiner SHA-256-Datei aktualisiert.

Das vollständige ZIP entpacken und die EXE gemeinsam mit dem Ordner `Daten` belassen. Die SHA-256-Datei gehört jeweils genau zur gleichnamigen EXE beziehungsweise ZIP-Datei.

Die Anwendungsversion bleibt 9.9.0; bereits installierte 9.9.0-Builds bekommen für diesen Austausch keinen neuen automatischen Versionshinweis.

Der aktuelle Quellcode wird separat in `Dragontools-Public` gepflegt. Frühere Release-Hinweise bleiben historisch erhalten.

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Downloads und Quelltext gewähren keine darüber hinausgehenden Nutzungsrechte. Mitgelieferte Laufzeitbibliotheken unterliegen ihren jeweiligen Lizenzen.
