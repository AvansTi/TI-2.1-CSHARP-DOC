>> ### Opgave 2.2 File IO
>> In deze opdracht ga je enkele gegevens van je systeem wegschreven naar een file. Maak een nieuw console project aan en:
>>
>> Ga na m.b.v. `Console.WriteLine(…)` dat je in System.Environment enkele statische properties hebt om:
>>
>> * De computernaam
>> * Besturingssysteem (os versie)  
>> * Aantal processoren in je systeem
>> * Username (inlognaam)
>>
>> Daarnaast heb je toegang tot enkele folder locaties: 
>>
>> * `CurentDirectory`
>> * `SpecialFolder.MyPictures` (en vele andere speciale folders)
>>
>> Voeg bovenstaande eigenschappen toe aan en `List<string>` mySystemProperties structuur en schrijf deze `list<string>` op twee manieren naar een tekstfile: 
>>
>> * `File.WriteAllLines(padnaam, mySystemProperties)` 
>> * `File.WriteAllText(padnaam, tekst)` In dit geval moet je zelf de `list<string> myProperties` tot één lange string omvormen. Gebruik hiervoor de methode `string.Join(…)`
>> * Lees de resulterende tekstfile in m.b.v. de tegenhangers `File.ReadAllText()` en `File.ReadAllLines()` 
>>
>> Test je programma!
>{: .exercise}