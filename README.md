# Eigenes Webseiten-Projekt


## Aufbau einer Seite
- **Kopfbereich** mit Titel oder Name
- **Einführung** mit kurzem Überblick oder großes Bild/Galerie
- **Hauptinhalt** mit Informationen
- **Kontakt oder Abschlussbereich**
- **Fußbereich** mit Zusatzinfos

## Grundlegende Entscheidung
- One-Pager
- mit Untersseiten


## Projekt
Überlegt euch eine Webseite, auf die ihr Lust habt.

- Welches Thema?
- Was soll auf der Seite sein?
- Überlegt ihr euch wie ihr diese Inhalte umsetzen könnt
    - Braucht ihr noch zusätzliches Wissen -> fragt mich oder Chatbots

- startet mit einer kleinen Version, die im Browser funktioniert
- erweitert sie anschließend Schritt für Schritt
- schaut regelmäßig im Browser nach, was sich verändert hat
- ihr dürft KI und bisher unbekannte Techniken als Hilfe nutzen



Es geht heute nicht darum, eine perfekte Webseite abzugeben. Nutzt die Zeit, um selbstständig etwas zu bauen, Dinge auszuprobieren und Spaß damit zu haben.



## Git-Workflow

Klont euer Projekt per SSH und wechselt auf den bereits vorhandenen Branch `solution`. Ersetzt `DEIN-PROJEKT` durch den Namen eures Kurs-Repositories:

```bash
git clone git@github.com:ctf-26d/DEIN-PROJEKT.git webprojekt
cd webprojekt
git switch solution
```

Arbeitet auf `solution`. Speichert eure Fortschritte regelmäßig mit einem Commit und pusht sie zurück ins Kurs-Repository (`origin`):

```bash
git add .
git commit -m "Projekt erweitert"
git push origin solution
```

### Optional: eigenes Projekt veröffentlichen

Erstellt in eurem eigenen GitHub-Account ein **öffentliches, leeres Repository** – ohne README, Lizenz oder `.gitignore`. Ersetzt die Platzhalter und verbindet es als zusätzliches Remote `deploy`. Pusht dann euren lokalen Branch `solution` dort auf den Branch `main`:

```bash
git remote add deploy git@github.com:DEIN-USERNAME/DEIN-REPO.git
git push deploy solution:main
```

Das Remote fügt ihr nur einmal hinzu. Bei weiteren Änderungen wiederholt ihr nach dem Commit beide Push-Befehle:

```bash
git push origin solution
git push deploy solution:main
```

Für GitHub Pages verwendet ihr euer öffentliches Repository und dessen Branch `main`.

![Git-Workflow: lokal auf solution arbeiten und zu origin sowie optional deploy pushen](Git-Workflow_%20Lokal%20und%20zwei%20GitHub-Repos.png)

## Abschluss

Vor dem finalen Push könnt ihr `hilfen.md` löschen und in der `README.md` eine kurze Beschreibung eures eigenen Projekts hinterlegen. Committet diese Änderungen, bevor ihr pusht.

- pusht euren Stand mit `git push origin solution` ins Kurs-Repository
- optional: veröffentlicht euer Projekt aus dem eigenen öffentlichen Repository mit GitHub Pages und teilt den Link im Slack


Auch unfertige und experimentelle Projekte dürfen veröffentlicht werden.
