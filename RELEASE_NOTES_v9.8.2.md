# DragonTools V9.8.2

DragonTools V9.8.2 ist ein Wartungs- und Datenbankupdate mit Fokus auf Dolby Vision, Jellyfin-Import, Mediathek-Suche, Renamer, Untertitel-Sidecars und robusterer Fehlerbehandlung.

## Highlights

- **Dolby-Vision-Crop korrigiert:** Ein Fehler wurde behoben, durch den die Dolby-Vision-RPU nach einem physischen Bild-Crop unter bestimmten Bedingungen ein zweites Mal gecroppt werden konnte. Die RPU wird jetzt korrekt auf das bereits verkleinerte Zielbild angepasst und anschließend erneut geprüft.
- **Jellyfin-12-Import überarbeitet:** Der Mediathek-Import wurde an die aktuelle Jellyfin-12-Datenbankstruktur angepasst. Jellyfin-Datenbanken werden weiterhin ausschließlich read-only über einen geprüften Snapshot eingelesen.
- **Mediathek auf Schema 6 erweitert:** Die interne DragonTools-Datenbank speichert jetzt deutlich mehr technische und inhaltliche Informationen.
- **Timestamp-Reparatur weiter gehärtet:** Die Reparatur arbeitet konsequenter fail-closed. Fehlerhafte Reparaturkandidaten ersetzen die Quelldatei nicht.

## Mediathek und Datenbank

- Originaltitel, Provider-IDs von TMDB, TheTVDB und IMDb, Genres, Tags, Studios, Filmreihen/Collections sowie schlanke Personenverknüpfungen werden gespeichert.
- Dateigröße, Laufzeit, Video-Profil, Streamdauer, Frameanzahl, Bildrate, Pixelformat, Bittiefe und relevante Farb- und HDR-Informationen werden umfangreicher erfasst.
- Der neue NFO-Lightscan prüft vorhandene Mediathek-Einträge gezielt auf zugehörige NFO-Dateien, ohne die komplette NAS erneut mit MediaInfo oder FFprobe zu analysieren.
- Nicht erreichbare Speicherpfade werden beim NFO-Lightscan als `unreachable` behandelt und nicht fälschlich als fehlend markiert.
- Die NFO-Konsistenzprüfung vergleicht Titel, Originaltitel, Jahr, Staffel, Folge und Provider-IDs aus vorhandenen NFO-Dateien mit den Mediathek-Daten. Abweichungen werden separat protokolliert, ohne die Datenbankwerte zu überschreiben.
- Die Mediathek-Suche wurde um Filter für NFO-Zustände, NFO-Abweichungen und weitere technische Informationen erweitert.
- Eigene SQL-Abfragen und normale Mediathek-Suchen können gespeichert werden.
- Die integrierte SQL-Hilfe zeigt Tabellen, Spalten, Datentypen und Beispielabfragen direkt aus dem aktuellen Schema.
- CSV-Exporte enthalten wieder den vollständigen Trefferbestand der aktuellen Suche. Das 500-Treffer-Limit gilt nur noch für die Anzeige in der Oberfläche.

## Renamer, Regeln und Sidecars

- Die Renamer-Fuzzy-Suche arbeitet jetzt mit mehreren konfigurierbaren Stufen. Standardmäßig werden nacheinander 60 Prozent, 45 Prozent und 30 Prozent Mindestübereinstimmung verwendet.
- Die neuen Fuzzy-Fallback-Grenzen werden dauerhaft über das Regelsystem gespeichert und bei älteren Regeldateien automatisch ergänzt.
- Einträge können unabhängig von der automatischen Erkennung gezielt als Film oder Serie gesucht werden.
- Suchbegriffe können manuell geändert werden; alle gefundenen Provider-Kandidaten bleiben sichtbar.
- Bei Treffern zeigt der Renamer direkt an, ob das Ergebnis von TMDB oder TheTVDB stammt.
- Schwächere Fallback-Treffer werden entsprechend gekennzeichnet und nicht wie sichere automatische Treffer behandelt.
- Der Regel- und Profil-Simulator zeigt zusätzlich zum geplanten Codec-, Audio-, Untertitel- und Zielpfadverhalten auch die berechnete Endauflösung.
- Wenn Auto-Crop erst während der Verarbeitung bestimmt werden kann, wird dies im Simulator kenntlich gemacht.
- Untertitel-Sidecars wurden erweitert: Textbasierte Untertitel können zusätzlich als SRT ausgegeben werden.
- Die Sidecar-Planung gilt einheitlich für Encode-, Remux-, DV-, HDR10+- und AV1-Pfade.

## Stabilität und Reparaturen

- Die Timestamp-Reparatur prüft Laufzeit, Streamanzahl und Lesbarkeit nach Reparaturversuchen erneut.
- Der FFmpeg-Fallback nutzt jetzt `+genpts/+igndts`, damit Dateien mit defekten DTS/PTS-Zeitstempeln näher am bewährten Batch-Fallback repariert werden.
- Verworfene Reparaturkandidaten können zur Fehleranalyse im Archiv `Timestamp_Reparatur` abgelegt werden.
- Fehlerhafte Reparaturkandidaten ersetzen die Quelldatei nicht.
- Defekte Timestamp-Fälle werden robuster behandelt und bei unplausiblen Ergebnissen konsequent verworfen.

## Dokumentation und Release-Prüfung

- Help, README, technisches Handbuch, PDF-Handbuch, Changelog und `Hilfe -> Über` wurden auf den aktuellen Funktionsstand gebracht.
- Die Release-Prüfung erkennt veraltete Dokumente im fertigen Build.
- Die Dokumentation beschreibt die neuen Datenbank-, Renamer-, Sidecar- und Reparaturfunktionen.

## Installation

1. `DragonToolsV9.8.2.zip` und die zugehörige `.sha256`-Datei herunterladen.
2. Die SHA-256-Prüfsumme kontrollieren.
3. Das ZIP in einen neuen Ordner entpacken.
4. `DragonToolsV9.8.2.exe` starten.
5. Benötigte externe Medienprogramme anhand von `TOOLS_INSTALLIEREN.txt` einrichten.

Das Windows-Paket enthält DragonTools samt Python-Laufzeit, aber keine externen Medienprogramme. FFmpeg/FFprobe, MKVToolNix, GPAC/MP4Box, dovi_tool, hdr10plus_tool und MediaInfo müssen aus den jeweiligen offiziellen Quellen bezogen und in DragonTools hinterlegt werden.

## Updatehinweise

- Laufende Aufgaben vor dem Wechsel beenden.
- Den bisherigen Programmordner nicht direkt überschreiben.
- Persönliche Einstellungen und Profile vorher sichern.
- Ein bereits installiertes 9.8.2 erkennt diesen aktualisierten 9.8.2-Build nicht automatisch als neuer, weil die Versionsnummer gleich bleibt.
- Eine Windows-SmartScreen-Warnung kann bei einer noch nicht digital signierten Anwendung auftreten.

## Dateien

- `DragonToolsV9.8.2.zip`
- `DragonToolsV9.8.2.zip.sha256`
