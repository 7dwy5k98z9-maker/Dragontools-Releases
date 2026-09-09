# Release-Checkliste

1. Versionsnummer in DragonTools erhöhen.
2. Gesamte Testsuite und Release-Validierung erfolgreich abschließen.
3. Öffentlichen Quellstand auf private Daten prüfen.
4. Windows-Anwendung frisch bauen und auf einem sauberen System testen.
5. Vollständigen Anwendungsordner als ZIP verpacken.
6. SHA-256-Prüfsumme erzeugen.
7. GitHub Release mit einem Tag wie `v9.9` anlegen.
8. Release-Hinweise, ZIP und Prüfsumme anhängen.
9. Release zunächst als Entwurf prüfen.
10. Erst danach als stabiles Release veröffentlichen.

Die in DragonTools eingebaute Updateprüfung findet nur eine Version, die höher als die installierte Version ist. Für Version 9.8 muss der erste Test daher beispielsweise `v9.9` tragen.
