# Fachinformatik
Anki Deck FIAE AP2

Anki Download: https://apps.ankiweb.net/#download

Folgendes Plugin für Anki wird benötigt:
https://github.com/Stvad/CrowdAnki

## Workflow (Details unten)
### Initial
Repo klonen, Ordner in Anki importieren.
### Aktuelle Version ziehen
Repo pullen, Ordner in Anki importieren
### Karten ändern/hinzufügen
Über den Anki Client (Deck auswählen und dann Add oder einfach editieren wenn man eine Karte offen hat)
### Geänderte/neue Karten in die Repo pushen
Zuerst Repo pullen, dann in Anki importieren (Anki merged die Karten), dann das Deck als CrowdAnki JSON exportieren und Dateien im Repo Ordner dabei überschreiben, dann pushen.

## To start working on the deck your collaborators need to
1. Install git

2. `git clone https://github.com/cptwtf/Fachinformatik.git`

3. Import the deck.
  (In Anki client use File -> "CrowdAnki: Import from disk" and choose **repo folder**)

## How to upload changes
### When you or one of your collaborators want to upload changes you've made to the GitHub, you need to:

#### Get the latest changes from the GitHub:

1. `git pull`
2. Import the deck in Anki client to combine changes you've made with the changes other people have made. Anki client use File -> "CrowdAnki: Import from disk" and choose **repo folder**.


3. Export (Anki client -> File -> Export -> Export Format (CrowdAnki JSON Representation) -> Include (Fachinformatik)) to the **repos folder parent** (example: repo is located at C:/repos/Fachinformatik then choose C:/repos/ as export location) to update JSON and media folder.

#### Add the changes to the repository:

`git add *`
`git commit -m "new updates"`
`git push`

If you just want to get latest changes from other people - you need to perform only steps 1 and 2.
