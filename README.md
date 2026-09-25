# DragonTools Releases

Öffentliche Downloadquelle von DragonTools unter dem Entwicklernamen **Dragon Developer**.

## Aktuell vorbereitet: DragonTools 9.8.6

Das Windows-Paket wurde am 25.09.2026 aus dem anonymisierten Public-Stand gebaut. Datenschutzprüfung, gezielte Release-Tests und die integrierte Build-Validierung wurden erfolgreich abgeschlossen. Die Build-Validierung meldete **0 Fehler und 0 Warnungen**. Details stehen in `RELEASE_NOTES_v9.8.6.md`.

- Paket: `artifacts/DragonToolsV9.8.6-win64.zip`
- Prüfsumme: `artifacts/DragonToolsV9.8.6-win64.zip.sha256`
- Größe: 777514206 Bytes
- SHA-256: `1e91d2459309b2faee6b32b11bb1973d7c16b7f79f4836fca4dfde0e8bb07350`

ZIP-Integrität und SHA-256 wurden nach der Erstellung erneut geprüft. Das ZIP enthält die EXE und den vollständigen erforderlichen Datenordner. Externe Medienwerkzeuge werden entsprechend der bisherigen Public-Paketierung separat eingerichtet; `TOOLS_INSTALLIEREN.txt` liegt bei.

## Veröffentlichung und Installation

ZIP und SHA-256 sind lokale Release-Artefakte und werden gemäß `.gitignore` nicht als Git-Dateien eingecheckt. Für die Veröffentlichung beide Dateien gemeinsam an ein GitHub Release mit dem Tag `v9.8.6` anhängen. Ein Git-Push allein veröffentlicht kein Release und löst noch keinen Updatehinweis aus.

Zum Installieren die Prüfsumme prüfen, das ZIP in einen neuen Ordner entpacken und die EXE zusammen mit ihrem Ordner `Daten` belassen. Eigene Einstellungen und Regeln vor einem Update sichern.

Der Quellcode wird separat in `Dragontools-Public` gepflegt. Dieses Repository enthält ausschließlich Release-Hinweise und Veröffentlichungsinformationen. Frühere Release-Hinweise bleiben historisch erhalten.

## Bekannte Grenzen

Abbruch ist kooperativ. Der Windows-Neustartschutz ist keine garantierte Sperre gegen erzwungene Update-Neustarts. Die automatisierten Tests ersetzen keine vollständige Hardware-Encoder-/Medienmatrix oder interaktive GUI-Abnahme.

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Die Veröffentlichung von Download oder Quelltext allein gewährt keine darüber hinausgehenden Nutzungsrechte.

## Aktualisierter Stand vom 25.09.2026

Der erneute Abgleich enthält die Patches BA, BB und BC: getrennte Original-Timingreferenzen, manuelle Episodenwahl und Datei-Einstellungen für Mehrfachauswahl. Alle 12 gezielten Regressionstests bestehen. Das anonymisierte Windows-Paket wurde neu gebaut und ZIP sowie SHA-256 erneut geprüft. Die Versionsnummer bleibt 9.8.6.
