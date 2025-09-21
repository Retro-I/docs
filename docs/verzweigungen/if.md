# If

## Theorie
Die If-Anweisung ist die einfachste Möglichkeit etwas wärehnd des Programmablaufs zu überprüfen und aufgrund dieses Ergebnisses weitere Anweisungen vorzunehmen.

Die If-Anweisung beinhaltet zwei Teile:
- Prüfungsteil
- Anweisungsblock

```cs
if (BEDINGUNG == true)
{
    // ANWEISUNG
}
```

## Beispiel
Es ist zu prüfen, ob eine Person minderjährig ist. Ist die Person minderjährig, soll eine entsprechende Ausgabe auf der Konsole erfolgen:

```cs
int alter = 16;

if (alter < 18)
{
    Console.WriteLine("Die Person ist minderjährig!");
}
```

??? quote "Ausgabe"
    ``` text
    Die Person ist minderjährig!
    ```
