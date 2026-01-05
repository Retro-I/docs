# Schaltplan

Für die technisch Versierten, gäbe es hier auch einen Schaltplan vom `Retro.I` wie wir den Radio aufgebaut haben.

## Schaltplan Retro.I
![Ansicht_vorne](../assets/schaltplan/Schaltplan.jpg)

## GPIO-Pin Belegung
| PIN | Farbe | Verwendung |
|-----|-------|------------|
| 1   | <span style="color:red">ROT</span> | 3,3V (Lüfter) |
| 2   | <span style="color:blue">BLAU</span> | 5V (Drehregler) |
| 4   | <span style="color:red">ROT</span> | 5V (Touch-Display) |
| 6   | <span style="color:black">SCHWARZ</span> | GROUND (Touch-Display) |
| 7   | <span style="color:gold">GELB</span> | CLK (Drehregler Bass UP) |
| 8   | <span style="color:orange">ORANGE</span> | DT (Drehregler Bass DOWN) |
| 9   | <span style="color:black">SCHWARZ</span> | GROUND (Lüfter) |
| 14  | <span style="color:black">SCHWARZ</span> | GROUND (Taster Shutdown) |
| 16  | <span style="color:red">ROT</span> | Daten (Taster Shutdown) |
| 19  | <span style="color:green">GRÜN</span> | Daten (LED-Streifen) |
| 20  | <span style="color:white; background:black; padding:2px">WEISS</span> | GROUND (LED-Streifen) |
| 23  | <span style="color:gold">GELB</span> | CLK (Drehregler Höhen UP) |
| 24  | <span style="color:orange">ORANGE</span> | DT (Drehregler Höhen DOWN) |
| 30  | <span style="color:purple">LILA</span> | GROUND (Drehregler) |
| 31  | <span style="color:green">GRÜN</span> | CLK (Drehregler Volume UP) |
| 32  | <span style="color:gold">GELB</span> | DT (Drehregler Volume DOWN) |
| 33  | <span style="color:orange">ORANGE</span> | SW (Drehregler Volume An/Aus) |
| 39  | <span style="color:black">SCHWARZ</span> | GROUND (Button Trinkspruch) |
| 40  | <span style="color:red">ROT</span> | Daten (Button Trinkspruch) |

![GPIO_pin_mapping](../assets/schaltplan/gpio_pin_mapping.png)
