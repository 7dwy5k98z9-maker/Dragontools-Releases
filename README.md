# DragonTools Releases

Öffentliche Downloadquelle von DragonTools unter dem Entwicklernamen **Dragon Developer**.

## Aktuell vorbereitet: DragonTools 9.8.3

Das Windows-Paket wurde am 15.09.2026 gebaut. Die vollständige Testsuite bestand mit **1.390 bestandenen Tests ohne Fehler oder Skips**, einschließlich zweier realer DV/HDR-Roundtrips. Details stehen in `RELEASE_NOTES_v9.8.3.md`.

- Paket: `artifacts/DragonToolsV9.8.3-win64.zip`
- Prüfsumme: `artifacts/DragonToolsV9.8.3-win64.zip.sha256`
- Größe: 189884483 Bytes
- SHA-256: `684d7ef2703505bb9f93350d5f786de7baa746b5733bf4d65a1cbfb60340dc7c`

ZIP-Integrität und SHA-256 wurden nach der Erstellung erneut geprüft. Das ZIP enthält die EXE und den vollständigen erforderlichen Datenordner. Externe Medienwerkzeuge werden entsprechend der bisherigen Public-Paketierung separat eingerichtet; `TOOLS_INSTALLIEREN.txt` liegt bei.

## Veröffentlichung und Installation

ZIP und SHA-256 sind lokale Release-Artefakte und werden gemäß `.gitignore` nicht als Git-Dateien eingecheckt. Für die Veröffentlichung beide Dateien gemeinsam an ein GitHub Release mit dem Tag `v9.8.3` anhängen. Ein Git-Push allein veröffentlicht kein Release und löst noch keinen Updatehinweis aus.

Zum Installieren die Prüfsumme prüfen, das ZIP in einen neuen Ordner entpacken und die EXE zusammen mit ihrem Ordner `Daten` belassen. Eigene Einstellungen und Regeln vor einem Update sichern.

Der Quellcode wird separat in `Dragontools-Public` gepflegt. Dieses Repository enthält ausschließlich Release-Hinweise und Veröffentlichungsinformationen. Frühere Release-Hinweise bleiben historisch erhalten.

## Bekannte Grenzen

Abbruch ist kooperativ. Der Windows-Neustartschutz ist keine garantierte Sperre gegen erzwungene Update-Neustarts. Die automatisierten Tests ersetzen keine vollständige Hardware-Encoder-/Medienmatrix oder interaktive GUI-Abnahme.

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Die Veröffentlichung von Download oder Quelltext allein gewährt keine darüber hinausgehenden Nutzungsrechte.
