# PJM Dokumentation git-Übung   

Dieses Dokument skizziert die Arbeitsschritte, die in der Aufgabe gemacht wurden. Außerdem werden kurz die verwendeten `git`-commands kurz umrissen. 

## Aufgabenstellung git basics 

Die Erzeugung eines neuen Git Repository auf dem lokalen Rechner erfolgt mit

`> git init`

Falls für den Benutzer auf dem System noch kein Username oder keine Email-Adresse für `git` festgelegt ist, erfolgt dies mit den Befehlen

`> git config user.name`

sowie 

`> git config user.email`

Beispiel: 

`> git config user.name "Werner Egermann"`

`> git config user.email es19m011@technikum-wien.at`


Die Erzeugung eines neuen `branches` erfolgt mit dem Befehl

> `git checkout -b <branchname>`

Alternativ dazu kann ein branch auch erzeugt werden mit dem Befehl 
 
> `git branch <branchname>`


Zunächst wird jedoch die Datei im git repo zum Index hinzugefügt mit 

`git add <filename>`

Nach dem Abändern des git-hooks `commit-msg` kann mit 

`git commit -m "<message text>"` 

der derzeitige Arbeitsstand im Index gespeichert werden. 

Nach mehreren commits auf dem branch `develop` wird ein weiterer branch `feature` erzeugt mit 

`git checkout -b feature` 

Auf diesem branch werden nun mehrere commits erzeugt. 


## Aufgabenstellung GitLab 

Leider hatte ich keinen Zugriff auf das FH-Gitlab. Daher habe ich Github genutzt und die Aufgabenstellung dort ausgeführt. 

Zunächst wird auf Github ein neues Projekt erstellt, dessen Namen ident ist mit dem Namen des lokalen repository. Das repository wird ohne README oder sonstigen Dateien erstellt, da diese später alle vom lokalen repo gepusht werden. 

Das auf Github erzeugte Projekt kann nun als `remote` zum lokalen `git`-Verzeichnis hinzugefügt werden mit 

`git remote add  origin <URL/to/repository.git>`

Als nächstes werden alle branches auf den git-Server geladen mit 
`git push origin --all`

`merge-request` wird auf Github `pull-request` genannt, die beiden Begriffe bezeichnen aber dasselbe. Dabei wird eine "Anfrage" gemacht, einen branch in einen anderen zu `mergen`, typischerweise einen develop-Branch in den master-Branch. 
Mit dem `merge-request` oder `pull-request` wird die Möglichkeit zu einem Code Review gegeben. Wenn das Code Review erfolgreich ist, kann "gemerged" werden, d.h. der eine Branch kann mit dem anderen zusammengeführt werden. 



## Möglichkeiten von GitLab hinsichtlich Projektmanagement 

- Auf Gitlab können verschiedene Rollen vergeben werden, und damit einhergehende Zugriffsrechte (z.B. Owner, Developer, Maintainer, ...). Somit können Rollen aus dem Projekt einigermaßen zugeordnet werden (z.B. Projektleiter = Owner). 
- Mehrere Personen können gleichzeitig verteilt an Dateien im gleichen Verzeichnis arbeiten, oder sogar an der gleichen Datei. 
- Es wird automatisch eine Dokumentation darüber erstellt, wie sich das Projekt entwickelt 
- Mithilfe von `merge-requests` kann ein Beitrag zur Qualitätssicherung geleistet werden 

