>>### Opgave 2.2
>>In deze opdracht ga je enkele gegevens van je systeem wegschreven naar een file. Maak een nieuw console project aan en:
>>
>><li>Ga na m.b.v. Console.WriteLine(…) dat je in System.Environment enkele statische properties hebt om:</li>
>>
>>
>><ul>
  >><li>De computernaam</li>
  >><li>Besturingssysteem (os versie) </li> 
  >><li>Aantal processoren in je systeem</li>
  >><li>Username (inlognaam)</li> 
>></ul>
>>
>>
>><li>Daarnaast heb je toegang tot enkele folder locaties: </li>
>><ul>
  >><li>CurentDirectory</li>
  >><li>SpecialFolder.MyPictures (en vele andere speciale folders)</li>
>></ul>
>>
>>Voeg bovenstaande eigenschappen toe aan en List<string> mySystemProperties structuur en schrijf deze list<string> op twee manieren naar een tekstfile: 
>><ul>
  >><li>File.WriteAllLines(padnaam, mySystemProperties) </li>
  >><li>File.WriteAllText(padnaam, tekst) In dit geval moet je zelf de list<string> myProperties tot één lange string omvormen. Gebruik hiervoor de methode string.Join(…)</li>
  >><li>Lees de resulterende tekstfile in m.b.v. de tegenhangers File.ReadAllText() en File.ReadAllLines() </li>
>></ul>
>>
>>Test je programma!
