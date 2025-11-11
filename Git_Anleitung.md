Git installieren:

		~sudo apt install git
		~git --version


Git config:

	So legst du deinen Namen und deine Email fest.
	
		~git config --global user.name "Dein Name"
		~git config --global user.email "Deine Email@email.com"

	Danach kannst du dir eine Übersicht anzeigen lassen mit:

		~git config --list
	
	und schauen ob es funktioniert hat.
	
	Mit alias kann man eine Variablie bzw. abkürzung für einen befehl erstellen.

		~git config --alias.<Variable> <Befehl>

	z.B.:	~git config --alias.i init

Git standard Befehle:

		~git help						//Hilfe

		~git init 						//Macht einen Reguleren Ordner zu einem Git Ordner	

		~git status						//Zeigt was in dem  Reposetory bisher passiert ist
		~git dif

		~git add						//Fügt Dateien der Stageing area zu (für Commit vormerken)
		~git add . 						//Fügt alle Datein die eine Änderung haben hinzu
		~git add <Dateiname>			//Fügt eine Speziefische Datei hinzu

		Git add muss jedes mal nach dem ändern einer Datei durchgefürt werden.
		
		~git rm --cached <DateiName>	//Entfernt Datein wieder 

		~git commit -m "Kommentar"		//Speichert den Dateistand in der Git-Historie

		~git show 						//Zeigt genau was sich geändert hat

		~git log						//Zeigt die verschiedenen commits

		~git restore					//Macht änderungen rückgänig

Git remote Reposetory:

	Wenn an einem online Git-Repo. gearbeitet wird solle man immer in einem neuen Branch arbetien um 
	bei einem Fehler nicht die Orginal-Datei zu beschädigen, jedoch muss man die Änderungen dann nochmal
	mergen.

		~git clone <Link>				//Kopiert ein Repo. von Git auf den PC
		
		-git checkout -b <Branch.Name> 	//Erstellt einen neuen Branch 
		
		~git branch						//Zeig alle Branches in dem Repo. an

		~git swicht <BranchName> 		//Wechseln zwischen den Branches & auf aktuellen Commit zurück gehen

		~git merge <BranchName> 		//Fügt Branches wieder zusammen

		~git push origin <BranchName>	//Lädt die geänderten Datein auf das online Git-Repo.

		~git pull 						//Lädt die geänderten Datein vom online Git-Repo. herunter

		~git checkout <Commit-ID>		//Gehe temprär auf den commit zurück

		~git reset --hard <Commit-ID>	//Dauerhaft auf Commit zurück springen

GitHub Desktop installieren:

	Erst muss PI-Apps installiert werden

		wget -qO- https://raw.githubusercontent.com/Botspot/pi-apps/master/install | bash

	Dann im Startmenu auf 	Accessories -> Pi Apps -> Programming -> 
							Github Desktop -> install

	https://pi-apps.io/install-app/install-github-desktop-on-raspberry-pi/



Allgemein:

		mkdir 							//Neuen Ordner erstellen
		pwd 							//Pfad anzeigen
		ls								//Listet alles im Verzeichnis
		cd								//gehe zu Ordner
		touch							//Erstellen einer neuen Datei


