>> ### Opgave 2.3 TcpClient en JSON
>> Leerdoelen:
>> * Werken met  `TcpClient` 
>> * Gebruik van JSON data 
>> * Gebruik maken van collecties (`List`, `Dictionary`, …)
>> * Serialisatie van data naar een file die je via `FileIO` opslaat op de computer. 
>> * (Reguliere expressie in C# specifiek voor onderstaande eerste alternatief) 
>>
>> * Ga na hoe je Newtonsoft.Json kunt installeren voor je project. Zie deze documentatie: [https://www.nuget.org/packages/newtonsoft.json/ ](https://www.nuget.org/packages/newtonsoft.json/)
>> * Maak een API key aan bij Open weather map (zie onderaan voor de API documentatie): [http://openweathermap.org/api](http://openweathermap.org/api). 
>> * Maak de volgende uitbreidingen op het voorbeeld uit de les: 
>> * In de API kun je ergens een lijst vinden van alle city ids waarvan je weerdata kunt opvragen. Zie:  [http://bulk.openweathermap.org/sample/](http://bulk.openweathermap.org/sample/) 
>>
>> Maak een getypeerde collectie aan van steden met hun weerdata. Je hebt hiervoor verschillende mogelijkheden. Hiervoor doe je per city id een request voor de actuele weergegevens. 
>>
>> * Sorteer de weerdata (een `List<T>`) op verschillende manieren en pas daarbij het implementeren van `interface IComparable<T>`  en abstracte `class Comparer<T>` toe in je applicatie 
>> * Schrijf de data naar een bestand toe. 
>> * Test je programma! 
>>
>> Alternatief: Je mag ook een andere open REST API gebruiken.
>{: .exercise}