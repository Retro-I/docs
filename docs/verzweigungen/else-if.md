# Else-If

## Theorie
Es gibt außerdem die Möglichkeit mehrere If- und Else-Anweisungen zu kombinieren. Dies ist mit der Else-If-Anweisung möglich.
Schlägt dabei eine If-Prüfung fehl, wird die Prüfung der nächsten Else-If-Anweisung durchgeführt.

## Beispiel
Zum vorherigen Beispiel ist zusätzlich zu prüfen, ob die Person ein Kind ist.

```cs
int alter = 10;

if (alter < 12)
{
    Console.WriteLine("Die Person ist ein Kind!");
}
else if (alter < 18)
{
    Console.WriteLine("Die Person ist ein Teenager!");
}
else
{
    Console.WriteLine("Die Person ist volljährig");
}
```
??? quote "Ausgabe"
    ``` text
    Die Person ist ein Kind!
    ```

!!! info "Erklärung"
	Da die Prüfung in Zeile 3 fehlschlägt, wird die Nächste Prüfung in Zeile 7 ausgeführt. Da diese Prüfungen erfolgreich ist, erscheint die entsprechende Ausgabe.
