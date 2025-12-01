# Setup
Hier findest du alle Informationen zum Setup-Skript ([`setup.sh`](https://github.com/Retro-I/Retro.I/blob/main/setup.sh))

Durch dieses Setup-Skript ist es möglich die Software des Radios ohne großen weiteren Aufwand zu installieren. \
Da die Installation mehrere Schritte benötigt und zusätzliche Software für die Lauffähigkeit notwendig ist, ist **JEDER** einzelne Schritt beschrieben.
Dies macht es möglich einen eventuell fehlschlagenden Schritt zu debuggen und zu verstehen, was überhaupt da so passiert. Außerdem kann jeder Schritt per Hand durchgeführt werden!
Näheres kann unter [Troubleshooting](#troubleshooting) nachgelesen werden.


## Durchführung Setup
Zur Durchführung des Setups sind die folgenden Schritte notwendig!

### Raspberry PI Image
Das Setup-Skript wurde lediglich auf einem `Raspberry PI OS (64-bit) "Debian Bookworm"` Image getestet.
??? note "Info"
    Dass das Setup-Skript auf anderen OS' funktioniert ist nicht ausgeschlossen, aber auch nicht garantiert!

Dieses Image kann über den **offiziellen** Raspberry-PI-Imager heruntergeladen und auf einer SD-Karte installiert werden.
Dabei ist folgendes zu beachten: \
* WLAN einrichten
* Geeigneten Benutzernamen für den Raspberry setzen

Optional bzw. **sehr** nützlich: \
* SSH aktivieren

### Projekt klonen
Wähle hierzu einen Ordner deiner Wahl. Wähle am besten einen Ort, den du schnell wieder findest. z.B. `/home/<USER>` oder `/home/<USER>/Documents`

Mit folgendem Command wird das Projekt geklont/heruntergeladen:
```commandline
git clone https://github.com/Retro-I/Retro.I.git
```
Im Normalfall, sollte `git` schon vorinstalliert sein. Sollte dies nicht der Fall sein, kann `git` mit folgendem Befehl installiert werden:
```commandline
sudo apt-get install git -y
```

### Setup.sh ausführen
Wechsle mit `cd Retro.I` in das Verzeichnis des Projekts und führe mit
```
./setup.sh
```
das Setup-Skript aus.


## Untergliederung
Das Setup-Skript ist in zwei Teile untergliedert:

### [Systemeinrichtung](systemeinrichtung.md)
Installiert Systemweite Software wie z.B. \
* Bildschirmtastatur
* `easyeffects`
* Konfiguriert den Splashscreen
* usw.

###  [App-Einrichtung](app-einrichtung.md)
* Richtet die virtuelle Python-Umgebung (`venv`) ein
* Installiert benötigte Pakete für `flet` und python
* usw.


## Troubleshooting
Eine konkrete Handlungsempfehlung gibt es für einen fehlschlagenden Schritt nicht! \
Dadurch, dass die einzelnen Schritte so gut es geht dokumentiert sind, sollte eine eigens durchgeführte Fehlerbehandlung gut möglich sein.

??? warning "Tipp"
    Während der Testphase konnten die sehr selten auftretenden Fehler durch erneutes Starten des Skripts gelöst werden! \
    Daher empfiehlt sich das Skript einfach erneut zu starten.


## Zusätzliche Hinweise
Auf [dieser Seite](hinweise.md) sind weitere nützliche Hinweise beschrieben wie z.B. Multitouch aktiviert werden kann.

??? info "Wichtig"
    Hierbei handelt es sich um Punkte, die **NICHT** automatisiert durch das Setup-Skript gelöst werden konnten!
