>>#### Opgave 1
>>
>> Tijdens de eerste opdracht maken we kennis met de basis concepten van C# zoals strucs, classes, formatting, etc.
>>
>> Opgave 1.1
>>Een `Time` waarde representeert een tijdstip van de dag zoals 10:05 of 00:45 als het aantal minuten vanaf middernacht (605 en 45 in deze voorbeelden). 
>>
>>Een `struct` van het type `Time` kan als volgt gedefinieerd worden:
>>
>>```cpp
>>public struct Time {
>>    private readonly int minutes;
>>    public Time(int hh, int mm) {
>>        this.minutes = 60 * hh + mm;
>>    }
>>
>>    public override String ToString() {
>>        return minutes.ToString();
>>    }
>>}
>>```
>>
>>Maak een Visual Studio C# console project met de naam *TestTime* en voeg bovenstaande `Time` definitie toe.
>>Voeg aan de `Main` methode enkele testwaarden toe van type `Time`, en print de `Time` waarden m.b.v. `Console.WriteLine`.
>>
>>Schrijf testcode om je  programma te testen.
>>De volgende onderdelen gaan verder met deze `Time` structuur.
>>
>>#### Opgave 1.2.1
>>In deze `Time struct` type, voeg je twee properties toe met alleen een getter:
>>- Voeg een property `Hour` toe om het aantal uur op te vragen. 
>>- Voeg een property `Minute` om het aantal minuten op te vragen.
>>
>>Tip: zie hoe dit in het voorbeeld van de les bij de class `Temperature` is gedaan
>>voor de properties: Celsius, Kelvin, Fahrenheit
>>
>>Bijvoorbeeld: `new Time(23, 45).Minute` geeft als waarde 45.
>>
>>#### Opgave 1.2.2
>>Wijzig de gegeven `ToString()` methode zodat deze een `Time` waarde formatteert
>>als hh:mm, bijvoorbeeld 10:05, in plaats van 605. Werk de methode uit op twee manieren:
>>- M.b.v. de `String.Format` methode.
>>- M.b.v. de sinds C# 6 manier van *string interpolatie*. 
>>
>>Ga ook na hoe je *number formattering* in C# kunt gebruiken, zodat uren en minuten met 2 cijfers worden weergegeven.
>>
>>Schrijf testcode voor beide manieren.
>>
>>*Extra uitdaging*: implementeer het interface `IFormattable` om een `Time` waarde
>>op verschillende manieren te kunnen afdrukken.
>>(Tip: gebruik de Visual Studio \<CTRL\> \<.\> om een stub te genereren voor het
>>implementeren van een interface.)
>>
>>**In de volgende oefening test je een verschil tussen classes en structs.
>>Op BB kun je een link vinden over *struct versus class*.
>>Lees dit eerst voordat je de volgende vraag beantwoord.**
>>
>>#### Opgave 1.3
>>Probeer een niet-statisch veld toe te voegen van type `Time` in de struct type `Time`.
>>Je zal merken dat dit problemen geeft. De vraag is nog waarom?
>>
>>Dit is dus recursieve definitie, in het geval van Time niet erg zinvol,
>>maar voor bijvoorbeeld een definitie van `Node` uit een `LinkedList` zou je een
>>dergelijke recursieve definitie wel willen. 
>>- Waarom kun je bij een recursief datatype in C# geen struct gebruiken?
>>- Waarom is een recursieve definitie voor een class wel mogelijk?
>>- Waarom kun je wel het volgende veld toevoegen aan de `struct Time`? 
>>`static Time noon = new Time(12,0);`
>>
>>#### Opgave 1.4
>>Maak het veld `minutes` van de struct-type Time `public` (en niet `readonly`)
>>in plaats van `private readonly`. 
>>
>>Test vervolgens de volgende code:
>>
>>```cpp
>>Time t1 = new Time(9,30);
>>Time t2 = t1;
>>t1.minutes = 100;
>>Console.WriteLine("t1={0} and t2={1}", t1, t2);
>>```
>>
>>Verklaar het resultaat. Wat is het verschil indien je van `Time` een class
>>in plaats van struct type maakt?
>>
>{: .exercise}