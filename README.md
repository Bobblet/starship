# starship




Starten der GraphHopper Routing API


Um die GraphHopper Routing API auf einem Lokalen Server unter Windows 10 zu starten müssen folgende Schritte durchgeführt werden:
1.	Öffnen der Kommandozeile 

2.	Dirigieren in das Verzeichnis, in dem die Dateien liegen

3.	Folgenden Code eingeben:

  a) Wichtig: Aufgrund der Datengrößenbegrenzung auf 25 MB konnte nur die osm.pbf-Datei von Bremen auf Github hochgeladen werden.     Demzufolge   muss man in dem folgenden Code den Namen der osm.pbf Datei ändern oder sich über folgenden Link den Berlin Datensatz runterladen:
https://download.geofabrik.de/europe/germany.html

  b)Berlin:
   java -Dgraphhopper.datareader.file=berlin-latest.osm.pbf -jar graphhopper-web-0.12-SNAPSHOT.jar server config-example.yml
   
   Bremen: 
   java -Dgraphhopper.datareader.file=bremen-latest.osm.pbf -jar graphhopper-web-0.12-SNAPSHOT.jar server config-example.yml

  
  

4.	Localhost starten via: http://localhost:8989
