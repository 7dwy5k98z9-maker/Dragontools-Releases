# DragonTools 9.8.2

## Änderungen

- Fehlerbehebung für den Dolby-Vision-Crop: Bei physisch gecroppten Video-Encodes konnte es vorkommen, dass die RPU doppelt gecroppt wurde.
- Nach dem FFmpeg-Crop werden die RPU-Level-5-Active-Area-Ränder auf das bereits verkleinerte Zielbild normalisiert.
- Die bearbeitete RPU wird vor der Injection auf ausschließlich nullgesetzte Level-5-Ränder geprüft.
- Bei gecroppten Dolby-Vision-Ausgaben wird die RPU nach dem finalen MKV- oder MP4-Mux erneut aus dem Bitstream extrahiert und bytegenau verglichen.
- Nicht prüfbare oder abweichende RPUs führen zum sicheren Abbruch, statt eine möglicherweise doppelt gecroppte Dolby-Vision-Datei auszugeben.
- Jellyfin-Datenbankimport für aktuelle Jellyfin-12.0-Datenbanken mit `BaseItems` und `MediaStreamInfos` angepasst.
- Importiert werden nur Filme, Serien, Staffeln, vorhandene Episoden und echte Videodateien; Personen-, Studio-, Genre-, Playlist-, Sammlungs- und Metadatenobjekte werden ausgeschlossen.
- Pfade, Serien-/Staffelstruktur, Laufzeit, Dateigröße, Container, Auflösung, Video-Codec, Video- und Gesamtbitrate werden übernommen.
- Audio- und Untertitelsprachen, Codecs, Kanäle, Forced-Kennzeichnung und verfügbare Bitraten werden gespeichert.
- Externe Untertitel werden in der DragonTools-Mediathek als externe Sidecars geführt, wenn Jellyfin sie entsprechend ausweist; ein echter Ordnerscan erkennt zusätzlich vorhandene Sidecars, NFO-Dateien und Trickplay-Ordner direkt im Dateisystem.
- Dolby Vision über RPU-/Profilfelder sowie HDR10+, HDR und SDR werden zuverlässig erkannt.
- Gleichwertige Windows-/UNC-Pfade werden dedupliziert; inkonsistente Jellyfin-DB-/WAL-Kopien werden vor dem Ersetzen der DragonTools-Mediathek abgelehnt.
- Timestamp-Reparatur arbeitet fail-closed: Fehler, unplausible Laufzeit, Vertragsverletzungen oder mögliche Streamverluste verhindern Ersetzen, Postprocessing und Verschieben.
- FFprobe und MediaInfo prüfen die Streamanzahl unabhängig; widersprüchliche Ergebnisse verwerfen den Reparaturkandidaten.
- Der verlustfreie FFmpeg-`+genpts`-Fallback steht auch zur Verfügung, wenn `setts` fehlt oder der erste Kandidat verworfen wurde.
- Der bekannte FFmpeg-EINVAL-Code `-22` beziehungsweise `4294967274` wird nur beim `+genpts`-Fallback und erst nach vollständigem Lesetest toleriert.
- Die DragonTools-Mediathek verwendet Schema 5 und speichert zusätzlich Dateigröße, Video-Profil, Streamdauer, Frameanzahl, Bildrate/-modus, Pixelformat, Bittiefe, Farbraum, Transferfunktion, Farbprimärwerte, Untertitel-Herkunft, NFO-Status und Trickplay-Status.
- Unplausibel kleine eingebettete Video-Bitraten können aus Streamgröße und Laufzeit neu berechnet werden.
- Die Suche unterstützt unbekannte Laufzeiten sowie Dateien unter einer Minute oder über fünf Stunden; CSV-Exporte enthalten die neuen technischen Felder.
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
- Ein bereits installiertes 9.8.2 erkennt diesen aktualisierten 9.8.2-Build nicht automatisch als neuer, weil die Versionsnummer gleich bleibt.
- Eine Windows-SmartScreen-Warnung kann bei einer noch nicht digital signierten Anwendung auftreten.

## Dateien

- `DragonToolsV9.8.2-win64.zip`
- `DragonToolsV9.8.2-win64.zip.sha256`
