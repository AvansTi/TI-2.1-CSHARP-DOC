>>### Opgave 1.2 Controlegetal (gebruik van bibliotheken)
>>
>>Bij het aanmaken van een nieuwe klant wordt een nieuw uniek rekeningnummer aangemaakt.
>>Dit nieuwe rekeningnummer moet voldoen aan de IBAN structuur.
>>De IBAN structuur bevat 2 cijfers ter controle van een geldig IBAN nummer.
>>
>>Maak een methode om dit controlegetal uit te rekenen en als een String
>>van 2 karakters terug te geven:
>>
>>```cpp
>>public static string BerekenControleGetal(string rekeningIdentificatie, string landcode)
>>```
>>
>>Tips:
>>- Maak voor berekeningen op grote gehele getallen gebruik van `System.Numerics.BigInteger`
>>Hiervoor moet je een referentie naar `System.Numerics` toevoegen aan je project.
>>Vervolgens een `using System.Numerics;` toevoegen in je class file waar
>>je `BigInteger` wil gebruiken.
>>- Een string omzetten naar een `BigInteger` kan m.b.v. `BigInteger.Parse()`
>>
>>Hieronder staat de uitleg voor de berekening van het controlegetal.
>>
>>**Controlegetal**
>>\[bron: [Wikipedia](https://nl.wikipedia.org/wiki/International_Bank_Account_Number#Structuur)\]
>>
>>Het controlegetal wordt verkregen door:
>>1.	de rekeningidentificatie te nemen
>>2.	er de landcode achter te plaatsen
>>3.	alle letters te vervangen door twee cijfers gebaseerd op de volgorde in het
>>Latijns alfabet beginnend met A=10, B=11, ..., Y=34, Z=35
>>4.	twee nullen toe te voegen aan het einde
>>5.	dan de rest bij delen door 97 nemen (mod 97)
>>6.	het controlegetal is 98 min deze rest
>>7.	als het controlegetal kleiner dan 10 is, een voorloopnul toevoegen
>>(controlegetal 1 wordt 01).
>>
>>Voorbeeld: voor een fictief Nederlands ING-rekeningnummer 1234567 is het
>>IBAN NLxx INGB 0001 2345 67 (zie hieronder). Het controlegetal wordt als volgt berekend:
>>
>>1.	INGB0001234567
>>2.	INGB0001234567NL
>>3.	1823161100012345672321 ("A" = "10", "B" = "11", "C" = "12", ... ,"I" = "18", ... ,"N"="23", enz).
>>4.	182316110001234567232100
>>5.	182316110001234567232100 mod 97 = 78
>>6.	98 - 78 = 20
>>
>>Het IBAN zal dus NL20INGB0001234567 zijn.
>>
>{: .exercise}