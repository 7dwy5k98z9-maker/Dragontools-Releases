# DragonTools 9.8.2

## Änderungen

- Dolby-Vision-Double-Crop bei physisch gecroppten Video-Encodes behoben.
- Nach dem FFmpeg-Crop werden die RPU-Level-5-Active-Area-Ränder auf das bereits verkleinerte Zielbild normalisiert.
- Die bearbeitete RPU wird vor der Injection auf ausschließlich nullgesetzte Level-5-Ränder geprüft.
- Bei gecroppten Dolby-Vision-Ausgaben wird die RPU nach dem finalen MKV- oder MP4-Mux erneut aus dem Bitstream extrahiert und bytegenau verglichen.
- Nicht prüfbare oder abweichende RPUs führen zum sicheren Abbruch, statt eine möglicherweise doppelt gecroppte Dolby-Vision-Datei auszugeben.
- Jellyfin-Import an aktuelle Datenbanken mit `BaseItems` und `MediaStreamInfos` angepasst.
- Importiert werden nur Filme, Serien, Staffeln, vorhandene Episoden und echte Videodateien; Personen-, Studio-, Genre-, Playlist-, Sammlungs- und Metadatenobjekte werden ausgeschlossen.
- Pfade, Serien-/Staffelstruktur, Laufzeit, Container, Auflösung, Video-Codec, Video- und Gesamtbitrate werden übernommen.
- Audio- und Untertitelsprachen, Codecs, Kanäle, Forced-Kennzeichnung und verfügbare Bitraten werden gespeichert.
- Dolby Vision über RPU-/Profilfelder sowie HDR10+, HDR und SDR werden zuverlässig erkannt.
- Gleichwertige Windows-/UNC-Pfade werden dedupliziert; inkonsistente Jellyfin-DB-/WAL-Kopien werden vor dem Ersetzen der DragonTools-Mediathek abgelehnt.
- Optionale GitHub-Updateprüfung aus V9.8.1 ist weiterhin enthalten.

## Installation

1. `DragonToolsV9.8.2-win64.zip` und die zugehörige `.sha256`-Datei herunterladen.
2. Die SHA-256-Prüfsumme kontrollieren.
3. Das ZIP in einen neuen Ordner entpacken.
4. `DragonToolsV9.8.2.exe` starten.
5. Benötigte externe Programme anhand von `TOOLS_INSTALLIEREN.txt` einrichten.

Das Windows-Paket enthält DragonTools samt Python-Laufzeit, aber keine externen Medienprogramme. Diese müssen von den jeweiligen offiziellen Projektseiten bezogen werden.

## Updatehinweise

- Laufende Aufgaben vor dem Wechsel beenden.
- Den bisherigen Programmordner nicht direkt überschreiben.
- Persönliche Einstellungen und Profile vorher sichern.
- Eine Windows-SmartScreen-Warnung kann bei einer noch nicht digital signierten Anwendung auftreten.

## Dateien

- `DragonToolsV9.8.2-win64.zip`
- `DragonToolsV9.8.2-win64.zip.sha256`
