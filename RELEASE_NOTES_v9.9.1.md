# DragonTools 9.9.1 – 12.10.2026

DragonTools verbindet Medienverarbeitung, Untertitelverwaltung und Benennung anhand von Metadaten. Version 9.9.1 enthält den aktuellen gemeinsamen Stand des privaten Projekts, des öffentlichen Quellcodes und des Windows-Pakets.

## Medienverarbeitung

### Bitmap-Untertitel und Laufzeit

Beim Einbrennen von PGS-Untertiteln läuft das Video nach dem Ende der Untertitelspur weiter. Der Overlay-Filter wiederholt das letzte Untertitelbild nicht. Dadurch entsteht beim Ende der Spur kein zusätzliches Bild mit einem weit entfernten Zeitstempel, das zuvor eine falsche Laufzeit und eine automatische Timestamp-Reparatur auslösen konnte. Die Bildrate, die B-Frame-Einstellungen und der zeitliche Abstand zwischen Audio und Video bleiben erhalten.

### Analyse und Verarbeitungsvorschau

Der MP4-Remux nutzt die vorhandene Medienanalyse und vermeidet zusätzliche vollständige Prüfungen vor dem Start. Die Videoliste zeigt die geplante Pipeline einschließlich Standard, HDR, Dolby Vision und kombinierter Verarbeitung. Die abschließende Prüfung der erzeugten Ausgabe bleibt Bestandteil der Verarbeitung.

## Untertitel

### Automatische Standardspur

Steht dieselbe Sprache an erster Stelle der Audio- und Untertitelregeln, wird bei anderssprachigem Wiedergabe-Audio ein ausgewählter Untertitel dieser Sprache als Standard gekennzeichnet. Ein regulärer Untertitel wird gegenüber einer Forced-Spur bevorzugt. Die Forced-Kennzeichnung bleibt erhalten. Die gemeinsame Auswahl gilt für Konvertierung, Strip-Only und Remux; exportierte Sidecars übernehmen die Standardkennzeichnung im Dateinamen.

### Formate und Spurzuordnung

Die Untertitelverwaltung berücksichtigt zusätzliche Textformate, prüft die einzufügenden Spuren und erhält deren Sprachangaben und Kennzeichnungen. Die Zuordnung orientiert sich an der tatsächlichen ffprobe-Spurtopologie. Nicht zugeordnete MediaInfo-Angaben verändern diese Topologie nicht.

## Renamer und Warteschlange

### Benennung und Serienbestand

Film- und Seriennamen werden im Hintergrund geändert. Die Dateiendung bleibt erhalten, vorhandene Zieldateien werden nicht überschrieben. Die Staffel- und Serienprüfung vergleicht erkannte Einträge mit ihrer gewählten Metadatenquelle und zeigt fehlende Staffeln, Specials und Folgen in einer exportierbaren Tabelle.

### Wiederherstellung und erneutes Hinzufügen

Die Journal-Wiederherstellung läuft beim Start im Hintergrund. Aus der Liste entfernte Dateien lassen sich erneut hinzufügen, sobald kein aktiver Auftrag sie mehr verarbeitet.

## Dokumentation und Windows-Paket

### Hilfe und Changelog

Hilfe, Handbuch und Versionsangaben sind auf 9.9.1 abgestimmt. Das Changelog beschreibt die technische Entwicklung nach Fachbereichen und Unterpunkten. JSON- und Textfassung enthalten dieselben Informationen.

### Installation

Das vollständige ZIP entpacken und die EXE zusammen mit dem Ordner `Daten` belassen. Die benötigten Python- und Qt-Laufzeitdateien sind enthalten. Externe Medienwerkzeuge werden separat eingerichtet; die Anleitung liegt als `TOOLS_INSTALLIEREN.txt` bei. Zu ZIP und EXE gehören eigene SHA-256-Dateien.

## Prüfung der Veröffentlichung

### Quellstand

Die vollständige Standardtestsuite bestand mit 5365 erfolgreichen Fällen. 13 Fälle wurden wegen optionaler Abhängigkeiten oder nicht verfügbarer Plattformfunktionen übersprungen; 24 DV/HDR-Integrationstests waren in diesem Lauf nicht ausgewählt. Die statische Codeprüfung, die öffentliche Datenschutzprüfung einschließlich der Dokumentation und die Quellvalidierung bestanden.

### Windows-Anwendung

Die erzeugte EXE bestand den echten Qt-Starttest. Die 18 App-Prüfpunkte ergaben keine Fehler. Sieben enthaltene Kernmodule stimmen mit dem veröffentlichten Quellstand überein. ZIP-Inhalt, CRC und SHA-256-Prüfsummen wurden geprüft; das Paket enthält keine externen Medienwerkzeuge. Zu ZIP und EXE liegen eigene Prüfsummen bei.
