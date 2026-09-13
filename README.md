# DragonTools Releases

Dieses Repository ist die öffentliche Downloadquelle für DragonTools und wird unter dem Entwicklernamen **Dragon Developer** gepflegt.

Fertige Windows-Pakete werden nicht als normale Git-Dateien gespeichert, sondern unter **Releases** veröffentlicht. DragonTools fragt beim Programmstart ausschließlich die öffentlichen Versionsinformationen des neuesten Releases ab. Ein Download oder eine Installation erfolgt nie automatisch.

Das vorbereitete aktuelle Release ist **DragonTools 9.8.2**. Es wird mit dem Tag `v9.8.2`, einem vollständigen Windows-ZIP und der zugehörigen SHA-256-Prüfsumme veröffentlicht.

Der aktuelle 9.8.2-Quellstand enthält neben der Dolby-Vision-Crop-Korrektur einen gehärteten Timestamp-Reparaturpfad mit FFmpeg `+genpts/+igndts` und Archivablage verworfener Reparaturkandidaten, das erweiterte Schema 6 der DragonTools-Mediathek und den kumulativen Technical Review Patch v4. Die Anwendung ist dabei weiter in fokussierte GUI-, Core- und Worker-Services zerlegt worden. Die realen DV-/HDR10+-Roundtrips erkennen lokal bereitgestellte Werkzeuge jetzt über die bekannten DragonTools-Toolordner und laufen regulär in der vollständigen Testsuite mit. Der synchronisierte Stand wurde mit **1.272 bestandenen Tests ohne Skips** geprüft.

Bei dieser Quell- und Repository-Synchronisierung wurde kein neues Windows-Paket erzeugt. Vorhandene ZIP- und SHA-256-Dateien bleiben deshalb unverändert. Weil die Versionsnummer unverändert bleibt, muss ein später neu gebautes 9.8.2-Paket samt Prüfsumme gemeinsam ersetzt beziehungsweise das Release neu erstellt werden. Eine installierte V9.8.2 erkennt einen anderen Build mit derselben Versionsnummer nicht als neueres Update.

## Für Anwender

1. Unter **Releases** die neueste stabile Version öffnen.
2. Das ZIP-Paket und die zugehörige `.sha256`-Datei herunterladen.
3. Die Prüfsumme kontrollieren.
4. Das ZIP in einen neuen Ordner entpacken.
5. Vorhandene persönliche Konfigurationen nur nach den jeweiligen Release-Hinweisen übernehmen.

Benötigte Medienprogramme sind nicht enthalten. Die Datei `TOOLS_INSTALLIEREN.txt` im ZIP nennt die offiziellen Downloadquellen und die Einrichtung in DragonTools.

## Veröffentlichungsregeln

- Release-Tags sind numerisch, zum Beispiel `v9.9` oder `v9.9.1`.
- Normale Updates werden als vollständige stabile Releases veröffentlicht, nicht als Entwurf oder Vorabversion.
- Jedes Release enthält das Windows-ZIP, eine SHA-256-Prüfsumme und verständliche Änderungshinweise.
- ZIP und Prüfsumme müssen aus demselben frisch geprüften Build stammen; nach jeder Änderung wird beides neu erzeugt.
- Quellcode wird im getrennten Repository `Dragontools-Public` gepflegt.
- Drittanbieterprogramme werden nur verteilt, wenn deren jeweilige Lizenz dies ausdrücklich erlaubt. Andernfalls verweist die Dokumentation auf die offiziellen Downloadquellen.

## Datenschutz

Dieses Repository darf keine privaten Namen, lokalen Pfade, Zugangsdaten, Protokolle, Einstellungen oder Testmedien enthalten.

## Lizenz

Für DragonTools wurde noch keine Open-Source-Lizenz erteilt. Die Veröffentlichung eines Downloads oder Quelltextes allein gewährt keine darüber hinausgehenden Nutzungsrechte.
