# Release-Checkliste

1. Versionsnummer in DragonTools erhöhen.
2. Gesamte Testsuite und Release-Validierung erfolgreich abschließen.
3. Öffentlichen Quellstand auf private Daten prüfen.
4. Windows-Anwendung frisch bauen und auf einem sauberen System testen.
5. Vollständigen Anwendungsordner als ZIP verpacken.
6. SHA-256-Prüfsumme erzeugen.
7. GitHub Release mit dem Tag `v9.8.1` und dem Titel `DragonTools 9.8.1` anlegen.
8. Release-Hinweise, ZIP und Prüfsumme anhängen.
9. Release zunächst als Entwurf prüfen.
10. Erst danach als stabiles Release veröffentlichen.

Die in DragonTools eingebaute Updateprüfung findet nur eine Version, die höher als die installierte Version ist. Das Release `v9.8.1` wird deshalb von V9.8 gefunden; in V9.8.1 selbst gilt es anschließend als aktuell.
