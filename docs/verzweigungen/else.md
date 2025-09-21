# Else

## Theorie
Eine Else-Anweisung ist <b>nur</b> in Verbindung mit einer If-Anweisung möglich!
Wie oben beschrieben, wird aufgrund eines Ergebnisses eine Anweisung ausgeführt oder eben nicht.
Schlägt die Prüfung bei einer If-Anweisung fehl und der Anweisungsblock wird <b>nicht</b> ausgeführt, kann im Gegenzug der Anweisungsblock der Else-Anweisung ausgeführt werden.

Dazu ist eine Erweiterung der If-Anweisung notwenig.

## Beispiel
Erweiterung: Ist die Person volljährig, soll ebenfalls eine entsprechende Ausgabe erfolgen

```cs
int alter = 20;

if (alter < 18)
{
    Console.WriteLine("Die Person ist minderjährig!");
}
else
{
    Console.WriteLine("Die Person ist volljährig!");
}
```

??? quote "Ausgabe"
    ``` text
    Die Person ist volljährig!
    ```
