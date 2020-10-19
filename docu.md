# PJM Dokumentation git-Übung   

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

Zunächst werden die gewünschten Dateien zum Index hinzugefügt mit 

`> git add <filename>` 

Diese Dateien werden jetzt von git getracked, d.h. es wird festgestellt, wenn sich die Datei ändert. 

Mit einem commit kann der momentane Zustand des Index ins git-repo gespeichert werden. 

`> git commit -m "commit-Nachricht"`

Die Erzeugung eines neuen `branches` erfolgt mit dem Befehl

`> git branch -b`

Nach dem ersten `commit` wird automatisch der `master`-branch erzeugt. 
Weitere branches erzeugt man entweder mit `git branch <branch-name>` oder mit `git checkout -b <branch-name>`. 

Die beiden branches develop und release werden erzeugt mit 

`> git checkout -b develop` 
`> git branch release`

Der Unterschied ist, dass die bereits eingecheckten Dateien in den develop-branch übernommen wurden, der release-branch aber leer ist. 




`> git branch release`
`> git branch release`
`> git branch release`
`> git branch release`
`> git branch release`
`> git branch release`
`> git branch release`
`> git branch release`



Zunächst wird jedoch die Datei im git repo zum Index hinzugefügt mit 

`git add <filename>`



## Aufgabenstellung GitLab 





git Hook 

