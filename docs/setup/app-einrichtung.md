# App-Einrichtung
## VENV einrichten
Mit dem Befehl
```
python -m venv "$RETROI_DIR/.venv"
```
wird venv als virtuelles Environment angelegt.\
In diesem werden später alle Python-Pakete installiert und müssten somit nicht direkt systemweit, sondern in dieser virtuellen Umgebung, installiert werden.
Zusätzlich, wird die `.bashrc` angepasst, damit bei jedem Start eines Terminals in den Projektordner gewechselt und die virtuelle Umgebung gestartet wird:
```
# venv for Retro.I
cd /home/pi/Documents/Retro.I
source /home/pi/Documents/Retro.I/.venv/bin/activate
```

## Installiere Pakete für alsaaudio
Für alsaaudio wird das Paket `libasound2-dev` benötigt:
```
sudo apt-get install libasound2-dev -y -qqq
```

## Installiere Pakete für flet-ui
Für flet-ui als UI-Framework werden zwei weitere Pakete benötigt:
```
sudo apt install libmpv-dev mpv -y -qqq
```
Zusätzlich muss ein Symlink erstellt werden, damit flet-ui richtig starten kann:
```
sudo ln -s -f "/usr/lib/aarch64-linux-gnu/libmpv.so" "/usr/lib/aarch64-linux-gnu/libmpv.so.1"
```

## Installiere Python-Pakete
Zuletzt müssen alle Python-Pakete aus der `requirements.txt` **in venv** installiert werden:
```
source "$RETROI_DIR/.venv/bin/activate" && pip install -r requirements.txt -q
```
