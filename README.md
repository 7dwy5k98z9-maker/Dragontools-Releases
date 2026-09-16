# DragonTools Releases

Öffentliche Downloadquelle von DragonTools unter dem Entwicklernamen **Dragon Developer**.

## Aktuell vorbereitet: DragonTools 9.8.4

Das Windows-Paket wurde am 17.09.2026 aus dem anonymisierten Public-Stand gebaut. Private und Public-Testsuite bestanden jeweils mit **1.449 Tests ohne Fehler oder Skips**, einschließlich realer DV/HDR-Roundtrips. Details stehen in `RELEASE_NOTES_v9.8.4.md`.

- Paket: `artifacts/DragonToolsV9.8.4-win64.zip`
- Prüfsumme: `artifacts/DragonToolsV9.8.4-win64.zip.sha256`
- Größe: 195174266 Bytes
- SHA-256: `f857f31a077521d646df1a84e13ef68b5dd1e506f845351bf096f85c410c81b2`

ZIP-Integrität und SHA-256 wurden nach der Erstellung erneut geprüft. Das ZIP enthält die EXE und den vollständigen erforderlichen Datenordner. Externe Medienwerkzeuge werden entsprechend der bisherigen Public-Paketierung separat eingerichtet; `TOOLS_INSTALLIEREN.txt` liegt bei.

## Veröffentlichung und Installation

ZIP und SHA-256 sind lokale Release-Artefakte und werden gemäß `.gitignore` nicht als Git-Dateien eingecheckt. Für die Veröffentlichung beide Dateien gemeinsam an ein GitHub Release mit dem Tag `v9.8.4` anhängen. Ein Git-Push allein veröffentlicht kein Release und löst noch keinen Updatehinweis aus.

Zum Installieren die Prüfsumme prüfen, das ZIP in einen neuen Ordner entpacken und die EXE zusammen mit ihrem Ordner `Daten` belassen. Eigene Einstellungen und Regeln vor einem Update sichern.

Der Quellcode wird separat in `Dragontools-Public` gepflegt. Dieses Repository enthält ausschließlich Release-Hinweise und Veröffentlichungsinformationen. Frühere Release-Hinweise bleiben historisch erhalten.

## Bekannte Grenzen

Abbruch ist kooperativ. Der Windows-Neustartschutz ist keine garantierte Sperre gegen erzwungene Update-Neustarts. Die automatisierten Tests ersetzen keine vollständige Hardware-Encoder-/Medienmatrix oder interaktive GUI-Abnahme.

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Die Veröffentlichung von Download oder Quelltext allein gewährt keine darüber hinausgehenden Nutzungsrechte.
