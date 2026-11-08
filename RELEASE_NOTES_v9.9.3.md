# DragonTools 9.9.3 – 08.11.2026

- Verkürzte Serientitel: Suchtexte ab drei Wörtern und zehn Zeichen werden zusätzlich mit gleich langen Wortabschnitten längerer Titel verglichen. Ab 85 % Teilübereinstimmung erscheinen passende Provider-Treffer als Fallback zur manuellen Prüfung; der Teiltreffer-Prozentsatz wird angezeigt.

- Umlautsuche: Bei Filmen werden alle erzeugten Schreibvarianten gesucht und die Provider-Ergebnisse zusammengeführt. Ein früher TheTVDB-Treffer verhindert damit nicht mehr den passenden TMDB-Treffer mit Umlauten. Doppelte identische Ergebnisse werden entfernt.

- Trefferbewertung: Ein übereinstimmendes Filmjahr gibt keinen pauschalen Bonus mehr auf die Titelähnlichkeit. Unterschiedliche Titel erhalten dadurch keine falschen 100 %. Ein abweichendes Jahr senkt die Bewertung weiterhin.

- Untertitel extrahieren: Alle Sprachen oder mehrere einzelne Sprachen wählen. Je Video werden alle Spuren der gewählten Sprachen extrahiert. Ist keine gewählte Sprache vorhanden, werden alle Untertitel extrahiert und der Fallback protokolliert. Alle Sprachen ist die Voreinstellung; eine leere Auswahl extrahiert ebenfalls alle.

- Film-Zielordner ändern: Entspricht der gewählte Ordner dem geplanten Filmordner einschließlich Jahr, werden die Dateien direkt darin gespeichert. Andernfalls wird der geplante Filmordner darunter angelegt. Beispiel: Film (2026) direkt verwenden oder unter Film den Unterordner Film (2026) anlegen. Serien behalten ihre Staffelstruktur.

Die vorhandene Ordnerstruktur des Windows-Pakets mit EXE und Daten-Unterordner bleibt erhalten.

## Prüfungen und Windows-Paket

Die vollständigen Standardtestsuiten bestanden:

- Privater Entwicklungsstand: `5745 passed, 16 skipped, 24 deselected in 445.56s (0:07:25)`
- Öffentlicher Quellstand: `5741 passed, 20 skipped, 24 deselected in 437.10s (0:07:17)`
- Zusätzliche native Windows-Fenstertests: `2 passed, 32 deselected in 1.09s`

Statische Syntax- und Namensprüfung, öffentliche Datenschutzprüfung und Quellvalidierung bestanden. Der endgültige Windows-Build bestand die Paketvalidierung und den Starttest der tatsächlichen EXE. Alle 934 enthaltenen Anwendungsmodule entsprechen dem öffentlichen Quellstand. Die einzige erwartete Paketwarnung betrifft den bewusst fehlenden Ordner für externe Medienwerkzeuge.

Das Handbuch behält seine 408 Seiten. Word-Quelle und PDF sind anonymisiert; alle Seiten wurden erneut gerendert und Text und Seitenaufteilung mit dem mitgelieferten PDF verglichen.

- Öffentlicher Quellstand: [533c263](https://github.com/7dwy5k98z9-maker/Dragontools-Public/commit/533c263e8a4440a62810fcf451834ea34464ad13)
- ZIP: `DragonToolsV9.9.3-win64.zip`
- Paketgröße: 208105927 Bytes, 455 Dateien
- ZIP-SHA-256: `7826a36837b4346928f73c84e1ba0a841388d77b8193e5580d390d3c397b370c`
- EXE-SHA-256: `f1a4b4e09cb7ba435673199b0300ee1c901af0646ff597f6b419bcaa655e6308`

ZIP-Inhalt, CRC und SHA-256 wurden geprüft. Externe Medienwerkzeuge werden separat anhand von `TOOLS_INSTALLIEREN.txt` installiert. Das Paket enthält die erforderlichen Python-/Qt-Laufzeitdateien. EXE und Ordner `Daten` müssen zusammenbleiben.
