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

## Prüfung und Paket

Die vollständige öffentliche Standardtestsuite bestand: `5658 passed, 20 skipped, 24 deselected in 466.06s (0:07:46)`. Die zwei nativen Windows-Neustartschutztests bestanden zusätzlich. Die statische Prüfung auf Syntaxfehler und undefinierte Namen bestand. Die öffentliche Datenschutzprüfung und die Quellvalidierung bestanden.

Das erhaltene Handbuch wurde aus Word exportiert und enthält 408 Seiten. Versionsangaben und Titelseitendatum sind auf 9.9.2 und den 23.10.2026 abgestimmt. 1401 kanonische Dateien entsprechen nach der Anonymisierung dem Entwicklungsstand. Alle 930 kompilierten Anwendungsmodule stimmen mit dem öffentlichen Quellcode überein.

Die finale EXE bestand den Laufzeit- und Qt-Starttest. Die App-Validierung ergab keine Fehler. Die einzige erwartete Warnung betrifft den bewusst fehlenden Ordner für externe Medienwerkzeuge. ZIP-Inhalt, CRC und SHA-256 wurden geprüft; externe Medienprogramme sind ausgeschlossen.

- ZIP: `DragonToolsV9.9.2-win64.zip`
- Größe: 214315722 Bytes, 455 Dateien
- ZIP-SHA-256: `259bc868c940751713603071cf6e3de51f83b27da523351989b2e6e52a5b7766`
- EXE-SHA-256: `55f658cc341d2e5f80e5d8f1e9c9ec069044a6f717a2fa069b1c53b612447ea1`

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Externe Medienprogramme anhand von `TOOLS_INSTALLIEREN.txt` separat installieren.
