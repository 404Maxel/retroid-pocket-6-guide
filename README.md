# Eigenes Webseiten-Projekt

Baut eine Webseite zu einem Thema, auf das ihr Lust habt. Überlegt euch, welche Inhalte ihr zeigen möchtet.

## Start

Klont euer Kurs-Repository per SSH und wechselt auf den bereits vorhandenen Branch `solution`. Ersetzt `DEIN-PROJEKT` durch euren Repository-Namen:

```bash
git clone git@github.com:ctf-26d/DEIN-PROJEKT.git webprojekt
cd webprojekt
git switch solution
```

Das HTML-Grundgerüst in [index.html](index.html) ist bereits mit [style.css](style.css) verknüpft. Baut darauf eine kleine Version, prüft sie im Browser und erweitert sie Schritt für Schritt.

Tipps zum Aufbau, Ideen und Links findet ihr unter [Hilfen und Inspiration](help/hilfen.md). Ihr dürft KI und neue Techniken als Hilfe nutzen.

## Fortschritte speichern

Arbeitet auf `solution`. Committet eure Zwischenschritte und pusht sie ins Kurs-Repository (`origin`):

```bash
git add .
git commit -m "Projekt erweitert"
git push origin solution
```

## Abschluss

Vor dem finalen Push könnt ihr die Hilfedateien in `help/` löschen und in der `README.md` euer Projekt kurz beschreiben. Committet diese Änderungen und pusht euren Stand wie oben zu `origin`.

## Optional: veröffentlichen

Erstellt in eurem eigenen GitHub-Account ein **öffentliches, leeres Repository** – ohne README, Lizenz oder `.gitignore`. Ersetzt die Platzhalter und fügt es einmalig als Remote `deploy` hinzu. Pusht euren lokalen Branch `solution` dort auf `main`:

```bash
git remote add deploy git@github.com:DEIN-USERNAME/DEIN-REPO.git
git push deploy solution:main
```

Bei weiteren Änderungen wiederholt ihr nach dem Commit `git push origin solution` und `git push deploy solution:main`.

Veröffentlicht euer öffentliches Repository mit GitHub Pages aus `main` und teilt den Link im Slack. Auch unfertige und experimentelle Projekte dürfen veröffentlicht werden.

![Git-Workflow: lokal auf solution arbeiten und zu origin sowie optional deploy pushen](assets/Git-Workflow_%20Lokal%20und%20zwei%20GitHub-Repos.png)
