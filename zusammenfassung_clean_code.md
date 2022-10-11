Code ist sauber, wenn er leicht zu verstehen ist - für jeden im Team. Sauberer Code kann auch von einem anderen Entwickler als dem ursprünglichen Autor gelesen und verbessert werden. Mit der Verständlichkeit kommen Lesbarkeit, Änderbarkeit, Erweiterbarkeit und Wartbarkeit.
_____________________________________

## Allgemeine Regeln
1. Befolge Standardkonventionen.
2. Halte es einfach. Einfacher ist immer besser. Reduziere die Komplexität so weit wie möglich.
3. Pfadfinderregel: "Verlasse den Zeltplatz sauberer als du ihn vorgefunden hast."
4. Finde immer die Ursache. Suche immer nach der Ursache für ein Problem.

## Gestaltungsregeln
1. Platziere konfigurierbare Dateien oder Defaults gut sichtbar, halte sie auf hohem Abstraktionsniveau und versteck sie nicht in einer kleinen Methode.
2. Polymorphismus statt if/else oder switch/case.
3. Trenne Multithreading-Code.
4. Vermeide Überkonfigurierbarkeit.
5. Verwende Dependency Injection.
6. Befolge das Gesetz der Demeter. Eine Klasse sollte nur ihre direkten Abhängigkeiten kennen. Das vermindert Kopplung und erhöht die Wartbarkeit. Mehr: https://de.wikipedia.org/wiki/Gesetz_von_Demeter

## Tipps zur Verständlichkeit
1. Sei konsistent. Wenn du etwas auf eine bestimmte Weise tust, dann tue alle ähnlichen Dinge auf dieselbe Weise.
2. Verwende erklärende Variablen, auf keinen Fall Variablen aus nur einem Buchstaben.
3. Kapsel Randbedingungen ein. Randbedingungen sind schwer zu überblicken. Lege die Verarbeitung für sie an einer Stelle ab.
4. Bevorzuge dedizierte Wertobjekte gegenüber primitiven Typen, z.B. absolute Pfade statt Strings.
5. Vermeide logische Abhängigkeiten. Schreib keine Methoden, deren korrekte Funktion von etwas anderem in derselben Klasse abhängt.
6. Vermeide negative Konditionale.

## Regeln für Namen
1. Wähle beschreibende und eindeutige Namen.
2. Mache eine sinnvolle Unterscheidung.
3. Verwende aussprechbare Namen.
4. Verwende durchsuchbare Namen.
5. Ersetze magische Zahlen durch benannte Konstanten. Mehr: https://de.wikipedia.org/wiki/Magische_Zahl_(Informatik)
6. Vermeide das Encoden. Verwende keine Präfixe und häng keine Typinformationen an.

## Regeln für Funktionen
1. Klein.
2. Eine Funktion macht nur eine Sache.
3. Benutze beschreibende Namen.
4. Bevorzuge weniger Argumente.
5. Funktionen sollen keine Nebenwirkungen haben.
6. Verwende keine Flag-Argumente. Teile Methoden in mehrere unabhängige Methoden auf, die ohne Flags aufgerufen werden können.

## Regeln für Kommentare
1. Versuche immer, dich im Code zu erklären.
2. Sei nicht redundant.
3. Füge nichts offensichtliches hinzu.
4. Verwende keine abschließenden Klammerkommentare.
5. Code der auskommentiert werden soll einfach entfernen.
6. Verwende Kommentare als Erklärung der Absicht.
7. Verwende Kommentare als Klarstellung des Codes verwenden.
8. Verwende Kommentare als Warnung vor Konsequenzen.

## Struktur des Quellcodes
1. Trenne Konzepte vertikal.
2. Zusammenhängender Code sollte vertikal dicht erscheinen.
3. Deklariere Variablen in der Nähe ihrer Verwendung.
4. Abhängige Funktionen sollten nahe beieinander liegen.
5. Ähnliche Funktionen sollten nahe beieinander liegen.
6. Platziere Funktionen in absteigender Richtung.
7. Zeilen kurz halten.
8. Verwende keine horizontale Ausrichtung.
9. Verwende Leerzeilen, um Zusammengehöriges zu verbinden und Unzusammenhängendes zu trennen.
10. Halte die Einrückung konsistent.

## Objekte und Datenstrukturen
1. Verstecke die interne Struktur.
2. Bevorzuge Datenstrukturen.
3. Vermeide hybride Strukturen (halb Objekt und halb Daten).
4. Objekte und Datenstrukturen sollten klein sein.
5. Objekte und Datenstrukturen sollten nur eine Sache tun.
6. Kleine Anzahl von Instanzvariablen.
7. Die Basisklasse sollte nichts über ihre Ableitungen wissen.
8. Es ist besser, viele Funktionen zu haben, als Code an eine Funktion zu übergeben, um ein Verhalten auszuwählen.
9. Bevorzuge nicht-statische Methoden gegenüber statischen Methoden.

## Tests
1. Eine Behauptung pro Test.
2. Lesbar.
3. Schnell.
4. Unabhängig.
5. Wiederholbar.

## Code-Smell (funktionierender Programmcode, der aber schlecht strukturiert ist)
Mehr: https://de.wikipedia.org/wiki/Code-Smell
1. Starrheit. Die Software ist schwer zu ändern. Eine kleine Änderung führt zu einer Kaskade von Folgeänderungen.
2. Fragilität. Die Software geht an vielen Stellen aufgrund einer einzigen Änderung kaputt.
3. Unbeweglichkeit. Teile des Codes können wegen der damit verbundenen Risiken und des hohen Aufwands nicht in anderen Projekten wiederverwendet werden.
4. Unnötige Komplexität.
5. Unnötige Wiederholungen.
6. Undurchsichtigkeit. Der Code ist schwer zu verstehen.

Übersetzt aus dem Englischen von Alexander Krug. 
Quelle/Source: https://gist.github.com/wojteklu/73c6914cc446146b8b533c0988cf8d29
