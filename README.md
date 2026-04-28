projekat: calculator-java -izvestaj
student:Hana Ćatović

1.softverske metrike
-ukupan LOC=214
    "Calculator.java"=188 linija
    "Start.java"=26 linija

2.statisticka analiza koda
Fajl             |linija| Zapazanje
Calculator.java  |6     |Globalno statičko polje finalResult (Thread-safety rizik). 
Calculator.java  |19    |Metoda ToString() krši Java konvenciju imenovanja.
Calculator.java  |37    |Nedostaje provera da li je string expression prazan pre pozivanja charAt(0).
Calculator.java  |90-184|Promenljiva Expression počinje velikim slovom (Naming convention).
Start.java       |1-26  |Glavna klasa direktno poziva Calculator bez adekvatnog hvatanja izuzetaka ili provere korisničkog unosa.
Start.java       |11    |Scanner se nepotrebno inicijalizuje unutar petlje (Resource management). 
Start.java       |17    |Poziv Calculator.Run bez try-catch bloka (Rizik od pucanja programa).
