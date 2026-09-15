# DragonTools 9.8.3

DragonTools 9.8.3 bündelt die seit 9.8.2 integrierten Review-Korrekturen und einen gezielten Stabilitäts-Patch für parallele Aufträge, Nachbearbeitung und sichere Dateitransaktionen.

## Highlights

- Verlässliche Warnungs- und Fehlerzustände: Ein verspäteter Erfolg der Nachbearbeitung kann die Auto-Move-Sperre nicht mehr aufheben.
- Eigene Prozesszuordnung je Hintergrundauftrag schützt parallel laufende Jobs vor fremden Abbrüchen und Timeouts.
- Späte Abbrüche werden vor dem finalen MP4-Commit und vor dem Löschen des Originals erneut geprüft.

## Fehlerbehebungen und Stabilität

- Statusübergänge werden synchronisiert und können einen terminalen Fehler oder eine Cleanup-Warnung nicht nachträglich herabstufen.
- Timeout, Pause und Abbruch verwenden die konkrete Prozessinstanz des jeweiligen Auftrags. Ein ausdrücklich ausgelöster Batch-Abbruch gilt weiterhin für den ganzen Batch.
- MP4- und DV-Ausgaben erhalten zusätzliche Schutzprüfungen an den Commit-Grenzen. Sidecar-Rollbacks und Recovery-Informationen bleiben bei unvollständiger Bereinigung erhalten.
- Bereits installierte DV-Ausgaben werden bei späteren Fehlern nicht als unvollständige temporäre Dateien behandelt.
- Quell-Trickplay wird vor destruktivem Ersetzen vorbereitet; Move-Recovery berücksichtigt umbenannte Video- und Begleitdateien.

## Technische und strukturelle Änderungen

- Gemeinsamer Ergebnisvertrag für Videoausgaben und Begleitdateien; konsistentere Weitergabe strukturierter Fehlerdetails.
- Weitere Aufteilung der DV-Remux-, Audio-Mux-, Ausgabevalidierungs-, Zeitzuordnungs-, Untertitel- und Metadatenlogik in Fachmodule unter Beibehaltung der bisherigen Fassaden.
- NFO-XML-Verarbeitung mit `defusedxml` gehärtet; SQL-Klassifikation der Mediathek trennt lesende Abfragen von Schreiboperationen konservativer.
- README, Hilfe, Über-Informationen, technische DOCX-Dokumentation und PDF-Handbuch auf den 9.8.3-Stand gebracht. Die öffentlichen Dokumente und Metadaten sind anonymisiert.

## Prüfung

- Vollständige Testsuite im anonymisierten Public-Projekt: **1.390 bestanden, 0 fehlgeschlagen, 0 übersprungen**.
- Darin enthalten: 20 gezielte neue Stabilitäts-Regressionsfälle und zwei echte DV/HDR-Integrationstests.
- Syntaxprüfung und Ruff-Prüfung auf Syntaxfehler bzw. undefinierte Namen erfolgreich.

## Hinweise für bestehende Nutzer

- Vorhandene Einstellungen und eigene Regeln vor dem Update sichern.
- Abbruch bleibt kooperativ. Bereits abgeschlossene atomare Dateisystemoperationen können nicht rückwirkend verhindert werden; an den geprüften Commit-Grenzen wird bei erkanntem Abbruch zurückgerollt.
- Der Windows-Neustartschutz ist keine garantierte Sperre gegen erzwungene Update-Neustarts und wurde mit diesem Patch nicht verändert.
- Die Tests ersetzen keine vollständige Hardware-Encoder- und Medienmatrix.

## Installation und Update

1. `DragonToolsV9.8.3-win64.zip` und die passende `.sha256`-Datei herunterladen.
2. SHA-256 prüfen und das vollständige ZIP in einen neuen Ordner entpacken.
3. `DragonToolsV9.8.3.exe` starten. Der zugehörige Ordner `Daten` muss bei der EXE bleiben.
4. Benötigte externe Medienwerkzeuge separat einrichten. Sie sind entsprechend der bisherigen Public-Paketierung nicht im ZIP enthalten; `TOOLS_INSTALLIEREN.txt` beschreibt die Einrichtung.

## SHA-256

Datei: `DragonToolsV9.8.3-win64.zip`

`684d7ef2703505bb9f93350d5f786de7baa746b5733bf4d65a1cbfb60340dc7c`
