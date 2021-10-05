# M306-Service
# Werkstattauftrag W07-Webmin

## Inhaltsverzeichnis:

### 1. Autoren, Versionierung des Dokumentes

### 2. Einfuehrung
#### 2.1 **Was kann die Software**
Webmin ist ein Werkzeug/Software mit dem man ein Linux Server mit einem Browser verwalten kann. So kann man in Webmin verschiedene Module installieren mit denen man dann z.B die User verwalten kann. Auch kann man verschiedene Server Daemons konfigurieren wie z. B einen Apache Webserver oder DNS.

#### 2.2 **Vorgesehener Zeitaufwand**
Unser Zeitbudget ist auf 7 Lektion beschränkt. Unser vorgesehener Zeitaufwand nutzt genau die 7 Lektionen aus. Eins unserer Ziele ist, diese 7 Lektionen nicht zu überziehen und allfällige aufgaben von zuhause zu erledigen.

#### 2.3 **Mögliche Risiken und Stolpersteine**
- Das grösste Risiko/Gefahr ist für uns das Versagen der Hardware, einerseit, wissen wir nicht in welchen zustand sich der Raspberry Pi befindet. Aus Erfahrung können wir auch sagen, dass das Netzwerk nicht immer Stabil ist, dies kann auch noch zu Problemen führen.
- Was auch zu einen Störungsfaktor werden kann, ist Git und Markdown selber. Wir beide sind relativ neu auf diesem Gebiet un müssen uns selbst noch richtig einarbeiten.


#### 3. **Benoetigte Hard- und Software**
**Hardware:**
Unsere Wichtigste Hardware ist der Raspberry Pi, auf diesem wird das Webmin installiert und Konfiguriert. Unsere eigene Laptops sind auch noch ein wichtiges Glied unsere Hardware, nachdem auf dem Raspberry Pi VNC installiert ist, brauchen wir keinen zusätzlichen Bildschirm mehr und wir können von unseren eigenen Notebooks den Raspberry Pi fernverwalten.
<br> 1x HDMI auf MikroHDMI stecker
<br> 1x Micro SSD als Festplatte für den Raspi

**Software:**
Die benötigte Software, welche wir genutzt haben, sind VNC und ein ISO-File für das Raspberry Pi OS. 
    <br>VNC, Virtual Network Computing,  ist eine Software, die den Bildschirminhalt eines entfernten Rechners auf einem lokalen Rechner anzeigt und im Gegenzug Tastatur- und Mausbewegungen des lokalen Rechners an den entfernten Rechner sendet <br>
        



- Hardware (Materialliste, Funktionalitaet)
- Software (Anforderungen, Firmware, OS-Image, ergaenzende SW-Packages, Abhängigkeiten, Funktionalitaet)

### 4. Installationsanleitung (Didaktisch reduzierte Anleitung. Lernende sollen eine eigene Lösungswege realisieren)
### 4. Installationsanleitung (für die Lehrperson)
Die Installation von Webmin erfolgt über die Kommandozeile und ist relativ einfach zu erledigen. Als aller erstes führen wir diesen Befehl aus:
````sudo apt-get install libnet-ssleay-perl libio-socket-ssl-perl````
 
Danach gehen wir auf die folgende Webseite

````https://sourceforge.net/projects/webadmin/files/webmin````

und suchen uns die neueste Version der minimale Version.
Zu meinem Zeitpunkt war die neueste Version 1.973. 
Im Command einfach die neueste Version einsetzen.

````cd````

````wget http://prdownloads.sourceforge.net/webadmin/webmin-1.973-minimal.tar.gz````
 
Das Tar Archiv dass wir nun heruntergeladen haben, entpacken wir mit folgendem Command.

````tar-zxvf webmin-1.973-minimal.tar.gz````

Jetzt wechseln wir in das Verzeichnis von Webmin und führen die Installation durch.

````cd webmin-1.973````
````sudo ./setup.sh````
 
Nun kommen im Shell ein paar Fragen die man alle auf Default lassen kann. Das Passwort muss man natürlich setzen. Nachdem die Installation fertig ist kann man die letzte Frage noch mit “Y” bestätigen damit Webmin automatisch beim start des Systems startet.
 
Mit diesen Daten kommt man auf die Webmin Webpage:
````http://hostname:10000/````
- Anweisungen verstaendlich und nachvollziehbar
- Keine fertigen Loesungsschritte aufzeigen
- Hilfestellung (Tipps, Quellen...)

### 5. Qualitaetskontrolle (Pruefen der Funktionalitaet mit Ablauf von Kommandos und entsprechenden Outputs)

### 6. Error-Handling
Bei der Installation hatten wir keine Probleme.

### 7. Quellen
- Eigene Dokumentation aus dem Modul 126.
- VNC für Raspi: https://www.realvnc.com/de/connect/download/viewer/raspberrypi/
- Raspberry Pi Os: https://www.raspberrypi.org/software/ 

### 8. OpenSource Lizenz
