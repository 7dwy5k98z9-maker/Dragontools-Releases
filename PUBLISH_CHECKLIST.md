# Release-Checkliste 9.8.7

Der aktuelle Auftrag erzeugt ausschließlich lokale Artefakte. Kein GitHub Release wird angelegt oder veröffentlicht.

1. Anonymisierten Quellstand 9.8.7 mit Datenschutzprüfung kontrollieren.
2. Gezielte Release-Tests, Paketvalidierung und Frozen-Runtime-Smoke ausführen.
3. Bekannte Abweichungen der vollständigen Testsuite in den Release-Hinweisen dokumentieren.
4. Windows-Anwendung frisch ohne externe Medienwerkzeuge bauen.
5. Vollständigen Anwendungsordner als `artifacts/DragonToolsV9.8.7-win64.zip` verpacken.
6. ZIP-Inhalt, CRC-Integrität und private Marker einschließlich kompilierter Module prüfen.
7. SHA-256 aus exakt diesem ZIP erzeugen und als gleichnamige `.sha256`-Datei ablegen.
8. Release-Hinweise und Repository-Dokumentation committen und pushen. ZIP und SHA bleiben entsprechend `.gitignore` lokal.

Für eine spätere Veröffentlichung müssen die vorhandenen Testabweichungen bewertet und ZIP sowie Prüfsumme gemeinsam an ein GitHub Release angehängt werden. Ein Git-Push allein veröffentlicht kein Release und löst keinen Updatehinweis aus.
