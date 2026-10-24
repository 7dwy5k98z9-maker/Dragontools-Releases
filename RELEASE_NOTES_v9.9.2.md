# DragonTools 9.9.2 – 23.10.2026

Die Version übernimmt den aktuellen Entwicklungsstand mit folgenden Verbesserungen:

- Konfigurierbare Standarduntertitel und verbesserte Erkennung der Audiosprache; Whisper-Aufträge werden bei paralleler Verarbeitung abgestimmt.
- Stabilere Serienzuordnung und TVDB-Suche, einschließlich ähnlicher Seriennamen und Jahresangaben.
- Verbesserte Verschiebeabläufe für lange Dateinamen und Aktualisierung der Mediathek nach reinen Verschiebeaufträgen.
- Fortschrittsanzeige beim Mediathekimport und dauerhafte Statusanzeige in der Warteschlange.
- Verbesserte Bestätigung von Laufzeiten und Auswertung von MakeMKV-Titeln.
- Korrigierte Werkzeugpfade, Start von Hilfsaktionen sowie Ausnahmebehandlung einzelner Aufträge.
- Verbesserte Pausen-, Beendigungs- und Windows-Neustartsteuerung.

Das öffentliche Windows-Paket enthält keine externen Medienwerkzeuge. Diese werden anhand von TOOLS_INSTALLIEREN.txt separat installiert. Python- und Qt-Laufzeitdateien bleiben Bestandteil des Pakets.

## Nachbesserung vom 24.10.2026

TVDB-Titelprüfung berücksichtigt hinterlegte Titel-Aliasse auch bei der Validierung der Detaildaten. Die Prüfung des Serienjahrs bleibt erhalten; alternative Staffelzählungen werden nicht zusätzlich ausgewertet.

## Prüfung des aktualisierten Pakets vom 24.10.2026

Die private Nachbesserung bestand 160 gezielte TVDB-, Metadaten- und Renamer-Tests. Die vollständige öffentliche Standardtestsuite bestand: `5665 passed, 20 skipped, 24 deselected in 306.74s (0:05:06)`. Statische Prüfung, öffentliche Datenschutzprüfung und Quellvalidierung bestanden.

Die finale Windows-EXE bestand die App-Validierung und den tatsächlichen Qt-/Laufzeit-Starttest. Alle 930 enthaltenen Anwendungsmodule entsprechen dem öffentlichen Quellstand. Die einzige erwartete Paketwarnung betrifft den bewusst fehlenden Ordner für externe Medienwerkzeuge. ZIP-Inhalt, CRC und SHA-256 wurden geprüft. Das eigenständige Handbuch bleibt erhalten.

- Öffentlicher Quellstand: [d8a7189](https://github.com/7dwy5k98z9-maker/Dragontools-Public/commit/d8a71895f0bef86afc2d54f2007339034c16791e)
- ZIP: `DragonToolsV9.9.2-win64.zip`
- Größe: 214317033 Bytes, 455 Dateien
- ZIP-SHA-256: `7f0c3f161bc80ddae949bcd3ea71694bde9e7b2b5dc508941c47116bc40de58f`
- EXE-SHA-256: `d364b95dbdc4bc04bb2d986da4d13a76fd46cc2dd205d41f561769f670a9554c`

Die Version bleibt 9.9.2; das vorhandene Paket wird durch den nachgebesserten Build ersetzt. Frühere lokale Paketdateien bleiben unter `artifacts/previous-20261024/` gesichert.
