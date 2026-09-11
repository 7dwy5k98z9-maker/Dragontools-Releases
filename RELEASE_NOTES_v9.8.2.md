# DragonTools 9.8.2

## Änderungen

- Dolby-Vision-Crop korrigiert: Bei physisch gecropptem Bildmaterial konnte die Dolby-Vision-RPU unter bestimmten Bedingungen erneut gecroppt werden. DragonTools passt die RPU jetzt auf das bereits verkleinerte Zielbild an und prüft sie nach dem finalen MKV- oder MP4-Mux erneut.
- Jellyfin-12-Import überarbeitet: Der Mediathek-Import ist an die aktuelle Jellyfin-12-Datenbankstruktur angepasst und arbeitet weiterhin ausschließlich read-only über einen geprüften Snapshot.
- Mediathek auf Schema 6 erweitert: Neben den bisherigen technischen Daten werden jetzt unter anderem Originaltitel, Provider-IDs von TMDB, TheTVDB und IMDb, Genres, Tags, Studios, Collections beziehungsweise Filmreihen sowie schlanke Personenverknüpfungen gespeichert.
- Technische Mediadaten erweitert: Dateigröße, Laufzeit, Video-Profil, Streamdauer, Frameanzahl, Bildrate, Pixelformat, Bittiefe sowie relevante Farb- und HDR-Informationen werden umfangreicher erfasst.
- NFO-Lightscan ergänzt: Bestehende Mediathek-Einträge können gezielt auf zugehörige NFO-Dateien geprüft werden, ohne die komplette NAS erneut mit MediaInfo oder FFprobe zu analysieren. Nicht erreichbare Speicherpfade werden als `unreachable` behandelt und nicht fälschlich als fehlend markiert.
- NFO-Konsistenzprüfung eingeführt: Titel, Originaltitel, Jahr, Staffel, Folge und Provider-IDs aus vorhandenen NFO-Dateien können mit den Mediathek-Daten verglichen werden. Abweichungen werden separat protokolliert, ohne die eigentlichen Datenbankwerte zu überschreiben.
- Mediathek-Suche deutlich erweitert: Neue Filter für NFO-Zustände, NFO-Abweichungen, Medientypen, Bereiche und technische Eigenschaften machen die interne Datenbank besser auswertbar.
- SQL-Funktionen ausgebaut: Eigene SQL-Abfragen und normale Mediathek-Suchen können gespeichert werden. Die integrierte SQL-Hilfe zeigt Tabellen, Spalten, Datentypen und Beispielabfragen direkt aus dem aktuellen Schema.
- CSV-Export korrigiert: Das 500-Treffer-Limit gilt nur noch für die Anzeige in der Oberfläche. CSV-Exporte enthalten wieder den vollständigen Trefferbestand der aktuellen Suche.
- Renamer-Fuzzy-Suche flexibilisiert: Die automatische Trefferauswahl arbeitet mit mehreren konfigurierbaren Stufen. Standardmäßig werden nacheinander 60 Prozent, 45 Prozent und 30 Prozent Mindestübereinstimmung verwendet.
- Renamer-Regeln erweitert: Die neuen Fuzzy-Fallback-Grenzen werden dauerhaft im Regelsystem gespeichert und bei älteren Regeldateien automatisch ergänzt.
- Renamer um manuelle Suche erweitert: Einträge können unabhängig von der automatischen Erkennung gezielt als Film oder Serie gesucht werden. Der Suchbegriff kann manuell angepasst werden, und alle gefundenen Provider-Kandidaten sind sichtbar.
- Provider im Renamer sichtbar: Gefundene Treffer zeigen direkt, ob sie von TMDB oder TheTVDB stammen. Schwächere Fallback-Treffer werden entsprechend gekennzeichnet und nicht wie sichere automatische Treffer behandelt.
- Regel- und Profil-Simulator verbessert: Zusätzlich zum geplanten Codec-, Audio-, Untertitel- und Zielpfadverhalten wird die berechnete Endauflösung angezeigt. Wenn Auto-Crop erst während der Verarbeitung bestimmt werden kann, wird das kenntlich gemacht.
- Untertitel-Sidecars erweitert: Neben den bisherigen Sidecar-Regeln können textbasierte Untertitel zusätzlich als SRT ausgegeben werden. Die Planung gilt einheitlich für Encode-, Remux-, DV-, HDR10+- und AV1-Pfade.
- Timestamp-Reparatur weiter gehärtet: Reparaturkandidaten werden konsequent fail-closed geprüft. Laufzeit, Streamanzahl und Lesbarkeit werden nach Reparaturversuchen erneut kontrolliert; fehlerhafte Kandidaten ersetzen die Quelldatei nicht.
- Release- und Dokumentationsprüfung verbessert: Help, README, technisches Handbuch, PDF-Handbuch, Changelog und `Hilfe -> Über` wurden auf den aktuellen Funktionsstand gebracht. Die Release-Prüfung erkennt außerdem veraltete Dokumente im fertigen Build.

## Installation

1. `DragonToolsV9.8.2-win64.zip` und die zugehörige `.sha256`-Datei herunterladen.
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

- `DragonToolsV9.8.2-win64.zip`
- `DragonToolsV9.8.2-win64.zip.sha256`
