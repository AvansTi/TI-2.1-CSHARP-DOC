>>### Gameserver
>>Voor het opzetten van een netwerk game heb je vaak een specifieke server nodig waarin naast specifieke gamelogic verwerkt zit. In deze gameserver gaat het om spellen met een tijdaspect waarbij twee of meer spelers steeds een vraag/puzzel krijgen en de server per vraag of puzzel bepaald welke speler als eerste het correcte antwoord geeft. (Denk aan spellen zoals: trivial pursuit, quiz spellen, vlotte geesten, halli galli,  game of Set,…) 
>>
>>#### A. Simpele game-server
>>Schrijf een TCP server die steeds: 
>>- wacht op twee spelers (eventueel te generaliseren naar een willekeurig aantal spelers, maar dan dien je wel na te gaan hoe de server weet wanneer het spel kan starten. Dus wanneer is de laatste speler toegevoegd?) 
>>- vervolgens in een aparte thread een spel opstart voor deze spelers.  
>>
>>Beschrijving simpel spel verloop:  
>>Tijdens een spelsessie krijgen de twee spelers tot een bepaald aantal punten: 
>>- steeds een som (bijvoorbeeld: wat is 56 * 12?) waarop het antwoord een getal (integer is) en
>>- zodra één van de spelers het correcte antwoord geeft wordt bepaald welke speler een punt erbij krijgt en
>>- vervolgens wordt de volgend som opgegeven.
>>
>>#### B. Trival pursuit of game of set server of...
>>Wijzig de logica van de server zodat deze:
>>- in de gamelogica niet een som genereerd maar puzzels/vragen volgens het trivial pursuit spel of game of set of ander spel. 
>>- een score volgens de spelregels van dit spel bij houdt. 
>>
>>In deze opdracht maak je een game server voor het spelen van het spel Set. De regels van dit spel worden hier uitgelegd: https://nl.wikipedia.org/wiki/Set_(kaartspel). Op de volgende site staat een dagelijkse set puzzel: http://www.setgame.com/set/puzzle 
>>Over dit spel is de nodige wiskundige achtergrond en statistieken beschreven. Voor de geïnteresseerde in de wiskundige achtergrond: kans op een Set in n kaarten en verder zijn er op internet enkele andere artikelen te vinden. 

 

 
