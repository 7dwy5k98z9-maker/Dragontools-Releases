# DragonTools 9.8.2

## Änderungen

- Dolby-Vision-Double-Crop nach einem physischen Video-Crop behoben.
- Bearbeitete RPUs werden auf nullgesetzte Level-5-Ränder geprüft und nach dem finalen MKV-/MP4-Mux erneut aus dem Bitstream gegengeprüft.
- Fehlerhafte oder nicht sicher prüfbare RPUs führen zum sicheren Abbruch.
- Jellyfin-Import unterstützt aktuelle `BaseItems`-/`MediaStreamInfos`-Datenbanken.
- Medienhierarchie, Laufzeit, Dateigröße, Container, Auflösung, Codecs, Bitraten, Sprachen sowie DV/HDR10+/HDR/SDR werden übernommen.
- Mediathek-Schema 6 speichert zusätzliche Profil-, Frame-, Farb-, Stream-, Provider-, NFO-, Trickplay- und Untertitelinformationen.
- Originaltitel, Provider-IDs, Genres, Tags, Studios, Collections/Filmreihen und schlanke Personenbeziehungen werden importiert.
- Externe Untertitel werden in der Mediathek geführt; ein lokaler Scan erkennt zusätzlich Sidecars, NFO-Dateien und Trickplay-Ordner im Dateisystem.
- NFO-Lightscan ergänzt vorhandene Mediatheken um NFO-Bestand und Konsistenzprüfung, ohne dafür einen vollständigen NAS-Medienscan zu erzwingen.
- Datenbanksuche, Bereichsfilter, Medientypfilter, gespeicherte Abfragen, SQL-Hilfe und CSV-Export wurden erweitert.
- Timestamp-Reparaturen werden vor dem Ersetzen vollständig gelesen und mit FFprobe sowie MediaInfo auf Streamverluste geprüft.
- Fehlerhafte oder widersprüchliche Reparaturkandidaten verhindern Ersetzen, Postprocessing und Verschieben.
- Ein verlustfreier `+genpts`-Fallback ergänzt den FFmpeg-`setts`-Pfad.
- Untertitel-Sidecars können zusätzlich zu internen Untertiteln erstellt werden; textbasierte Formate können optional als SRT-Sidecar ausgegeben werden.

## Installation

1. ZIP herunterladen und Prüfsumme kontrollieren.
2. In einen neuen Ordner entpacken.
3. `DragonToolsV9.8.2.exe` starten.
4. Benötigte externe Programme anhand von `TOOLS_INSTALLIEREN.txt` einrichten.

## Updatehinweise

- Vorhandene laufende Aufgaben zuerst beenden.
- Den bisherigen Programmordner nicht direkt überschreiben.
- Persönliche Einstellungen und Profile vor dem Wechsel sichern.
- Bei einem Austausch innerhalb derselben Version 9.8.2 erscheint für bereits installierte 9.8.2-Builds kein automatischer Updatehinweis.

## Dateien

- `DragonToolsV9.8.2-win64.zip`
- `DragonToolsV9.8.2-win64.zip.sha256`
