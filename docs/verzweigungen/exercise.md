# Übung
Gegeben ist eine Punktzahl einer Prüfung. Aufgrund dessen soll das Ergebnis der Prüfung ermittelt werden.

## Schritt 1
Ist die Punktzahl größer 50 ist die Prüfung bestanden und es soll das Ergebnis der Prüfung ermittelt werden.

??? success "Lösung"
    ``` cs
    int punktzahl = 60;

    if (punktzahl > 50)
    {
        Console.WriteLine("Du hast bestanden!");
    }
    ```

## Schritt 2
Erweiterung zu <a href="#schritt-1">Schritt 1</a>: Ist die Prüfung nicht bestanden, soll ebenfalls ein entsprechender Text auf die Konsole geschrieben werden.

??? success "Lösung"
    ``` cs
    int punktzahl = 40;

    if (punktzahl > 50)
    {
        Console.WriteLine("Du hast bestanden!");
    }
    else
    {
        Console.WriteLine("Du hast nicht bestanden!");
    }
    ```

## Schritt 3
Die Punktzahl soll nun in Schulnoten umgewandelt werden und entsprechend ausgegeben werden.
Die angefügte Tabelle zeigt die Aufteilung in Noten.

| Note | Punktzahl       |
|------|-----------------|
| 1    | 100 - 90        |
| 2    | 89 - 80         |
| 3    | 79 - 65         |
| 4    | 64 - 50         |
| 5    | Nicht bestanden |

??? info "Tipp"
    Es wird der "größer-gleich" Operator (>=) benötigt!


??? success "Lösung"
    ``` cs
    int punktzahl = 60;

    if (punktzahl >= 90)
    {
        Console.WriteLine("Du hast die Note 1");
    }
    else if (punktzahl >= 80)
    {
        Console.WriteLine("Du hast die Note 2");
    }
    else if (punktzahl >= 65)
    {
        Console.WriteLine("Du hast die Note 3");
    }
    else if (punktzahl >= 50)
    {
        Console.WriteLine("Du hast die Note 4");
    }
    else
    {
        Console.WriteLine("Du hast nicht bestanden");
    }
    ```
