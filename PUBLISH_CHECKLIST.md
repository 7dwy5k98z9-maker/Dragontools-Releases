# Release-Checkliste 9.9.0 – 08.10.2026

1. Den anonymisierten öffentlichen Quellstand abgleichen und Datenschutzprüfung ausführen.
2. Vollständige Standardtestsuite und Syntax-/Namensprüfung ausführen.
3. Windows-Anwendung aus dem öffentlichen Quellstand ohne externe Medienwerkzeuge bauen.
4. App-Bundle, kompilierte Anwendungsmodule und tatsächlichen EXE-Start prüfen.
5. EXE mit vollständigem `Daten`-Ordner unter `artifacts` ablegen und ihre SHA-256-Datei erzeugen.
6. Den vollständigen Anwendungsordner als `artifacts/DragonToolsV9.9.0-win64.zip` verpacken, ZIP-Inventar und CRC prüfen und die zugehörige SHA-256-Datei erzeugen.
7. Release-Dokumentation committen und pushen. Das bestehende GitHub Release `v9.9.0` mit ZIP und Prüfsumme aktualisieren; die zusätzlichen lokalen Dateien bleiben unter `artifacts` erhalten.
