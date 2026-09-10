# DragonTools 9.8.2

## Änderungen

- Dolby-Vision-Double-Crop nach einem physischen Video-Crop behoben.
- Bearbeitete RPU wird auf nullgesetzte Level-5-Ränder geprüft.
- Finale MKV- und MP4-Ausgaben erhalten eine zusätzliche RPU-Rückprüfung.
- Fehlerhafte oder nicht sicher prüfbare RPUs führen zum sicheren Abbruch.
- Jellyfin-Import unterstützt aktuelle `BaseItems`-/`MediaStreamInfos`-Datenbanken.
- Medienhierarchie, Laufzeit, Container, Auflösung, Codecs, Bitraten, Sprachen sowie DV/HDR10+/HDR/SDR werden übernommen.
- Nichtmedien, gleichwertige Pfaddubletten und inkonsistente Datenbankkopien werden ausgeschlossen.
- Timestamp-Reparaturen werden vor dem Ersetzen vollständig gelesen und mit FFprobe sowie MediaInfo auf Streamverluste geprüft.
- Fehlerhafte oder widersprüchliche Reparaturkandidaten verhindern Ersetzen, Postprocessing und Verschieben.
- Ein verlustfreier `+genpts`-Fallback ergänzt den FFmpeg-`setts`-Pfad.
- Mediathek-Schema 4 speichert Dateigröße sowie zusätzliche Profil-, Frame-, Farb- und Streamdaten.
- Laufzeitfilter finden unbekannte, auffällig kurze und über fünf Stunden lange Dateien.

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
