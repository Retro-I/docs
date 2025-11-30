# Zusätzliche Hinweise
## Probleme mit Scrollen
Es ist möglich, dass das Touch-Display mit dem Scrollen hat.\
Sollte das Display kein Scrollen unterstützen kann während der Installation ausgewählt werden, ob man einen Scrollbalken in der App anzeigen lassen möchte.\

Für Displays, welche Touch unterstützen kann es sein, dass der Screen anfangs kein Scrollen ermöglicht.\
Ich benutze einen Touchscreen von Luckfox, der über das DSI-Kabel angeschlossen ist.\
Um bei mir Scrollen zu ermöglichen, musste ich folgendes anpassen:

```
Start -> ... Preferences -> Screen Configuration -> Screens -> <JEWEILIGEN SCREEN AUSWÄHLEN> -> Touchscreen -> Mode -> Multitouch
```

## Bildschirmhelligkeit einstellen
Es ist möglich, dass dein Bildschirm/Touchscreen keine Helligkeitseinstellung unterstützt.\
Es wird mit folgenden Mitteln versucht die Helligkeit zu verändern.\
für DSI-Bildschirme:
* es werden alle `brightness` Dateien in den Ordnern `/sys/class/backlight/*` gesucht und gesetzt

für HDMI-Bildschirme:
* `xrandr --output HDMI-0 --brightness <WERT>`
* `xrandr --output HDMI-1 --brightness <WERT>`
