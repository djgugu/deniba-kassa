# deniba-kassa
Update 

1. Build tauri app

> npm run tauri-build

erzeugt 3 Dateien unter src-tauri/release/bundle/msi

* .msi
* .msi.zip
* .msi.zip.sig

2. Release erstellen

* Unter https://github.com/djgugu/deniba-kassa auf *Releases* klicken.
* Dann *Draft a new Release* klicken
* *Release Title*, *Description*, *Tag* eingeben. (Semantic versioning beachten)
* Die Datei mit der Endung .msi.zip hinzufügen und auf *Publish release* klicken

3. static.json updaten

* Unter https://github.com/djgugu/deniba-kassa auf *static.json* klicken
* Diese Datei bearbeiten (Bearbeitungs icon anklicken)
* Unter platforms->windows-x86_64->signature den Inhalt von der Endung .msi.zip.sig hinzufügen
* Das Versions Attribute sowohl in *static.json* als auch in *tauri.conf.json* unter package->version ändern



