>>### Eindopdracht week 1: Mini casus
>>
>>Met de volgende C# taalelementen ga je oefenen:
>>- Maak gebruik van één of meer datum/tijd typen: TimeSpan, DateTime, DateTimeOffSet
>>Zie ook op MSDN: [Choosing Between DateTime, DateTimeOffset, TimeSpan](https://msdn.microsoft.com/en-us/library/bb384267(v=vs.110).aspx)
>>- Gebruik ergens een enumerated type (Bijvoorbeeld voor filmtype)
>>- Maak ergens gebruik van een List\<t\> en de foreach-loop
>>- Maak ergens gebruik van ref en/of out parameters
>>- Maak gebruik van `Tuple` types, zoals `(int, string)`.
>>Hiervoor heb je de laatste versie van Visual Studio nodig en bij property
>>van het project moet de Target Framework >= 5 zijn.
>>- Probeer gebruik te maken van interface en/of overerving en
>>- Maak bij toepassing van overerving gebruik van checked type casts
>>
>>Werk een console applicatie uit voor bijvoorbeeld één van de volgende situaties:
>>
>>#### Optie 1. Bioscoop agenda
>>Maak een applicatie om voor een bioscoop een agenda van de actuele films te maken.
>>Van iedere filmvoorstelling wordt vastgelegd:
>>- titel
>>- tijdstippen dat de film draait
>>- tijdsduur in minuten
>>- type (2D, 3D, 3DLaser)
>>- leeftijdscategorie
>>
>>In de applicatie kan een overzicht van films worden weergegeven van een dag en kan er
>>gezocht worden naar een film. Ook kan de bioscoopagenda van een hele week getoond worden.
>>Maak de klassen: `FilmVoorstelling`, `enum FilmType`, `Agenda` en `TestAgenda`
>>
>>#### Optie 2. Facturering GSM abonnement
>>Een aanbieder van GSM abonnementen wil een factureringssysteem bouwen voor het
>>factureren van zijn klanten. Voor iedere klant wordt aan het eind van iedere maand
>>de kosten bepaald aan de hand van een lijst belsessies en het soort abonnement
>>dat deze klant heeft. Er zijn verschillende soorten abonnementen.
>>Een abonnement wordt bepaald door het aantal vrije belminuten, beltarief
>>per minuut en uiteraard de prijs van het abonnement.
>>Per belsessie wordt bijgehouden wanneer de sessie start, hoe lang de sessie duurt
>>en naar welk nummer gebeld wordt. Afhankelijk van dit tijdstip, duur en nummer
>>kan de kosten berekend worden van deze belsessie. Tevens wordt er een prijs
>>voor sms’en bepaald. Voor een klant wordt een opgegeven periode (maand of anders)
>>een factuur gemaakt, met ook een totaalprijs. 
>>
>>Maak o.a. klassen: `BelSessie`, `Factuur`, `Abonnement` en `FacturenSysteem`
>>
>{: .exercise}