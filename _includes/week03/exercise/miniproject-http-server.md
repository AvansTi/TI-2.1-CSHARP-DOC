>>### Miniproject http server
>> Voor het internet worden veel op tekst gebaseerde servers gebruikt. Een voorbeeld hiervan zijn de servers voor websites. Het tekstprotocol dat hiervoor wordt gebruikt heet http. Bij dit protocol maakt de client een verbinding, vraagt een bestand op, en wacht hierna tot dit bestand binnen komt. De server luistert op een serversocket (poort 80), wacht op verbindingen en als er een verbinding binnen komt gaat hij luisteren tot het bestand is opgevraagd. Hierna stuurt de server wat informatie, gevolgd door het bestand. 
>>
>>In het project staat een simpele http-client. Deze client kan verbinding maken met een http-server, een bericht versturen en de antwoorden terugkrijgen. De client zal verbinding maken met de server in het adres, hier een verzoek naartoe sturen voor een bestand, en het antwoord weergeven in het tekstveld. Het bericht dat de client stuurt is:
>>```
>>GET <bestandsnaam> HTTP/1.0 ↵ 
>>Host: <hostname> ↵ 
>>↵ 
>>```
>> Hierbij staat ↵ voor een lege regel (in C# een “\r\n”). Zodra de server dus 2 ↵ achter elkaar binnenkrijgt, kan dit bericht verwerkt worden, en kan er antwoord gegeven worden. De server zal dan eerst wat informatie over dit bestand sturen, en hierna de gegevens die zijn opgevraagd.
>>
>>#### a. Simpele HTTP-server 
>>
>> Schrijf een http-server die wacht op een verbinding (op poort 80), hierna wacht tot het verzoek van de client is ontvangen en hierna altijd vast de volgende informatie verstuurd: 
>>```
>>HTTP/1.0 200 OK↵ 
>>Content-type: text/plain↵ 
>>↵ 
>>Hallo, dit is mijn internetpagina met tekst 
>>```
>>Test ook of je http-server het doet door met je internetbrowser (Internet Explorer, Firefox, Chrome, Opera, Safari) te surfen naar http://localhost/ . Let erop dat de ↵ in C# voorgesteld worden met “\r\n”, en niet alleen met “\n” 
>>
>>#### b. Basis opzet voor HTTP file server
>> Maak op basis van deze bestandsnaam de volgende keuzes om terug te sturen: 
>> Als bestandsnaam gelijk is aan “pagina2” 
>>```
>>HTTP/1.0 200 OK↵ 
>>Content-type: text/html↵ 
>>↵ 
>>Dit is pagina 2 <a href="/">terug</a> 
>>```
>>Als bestandsnaam gelijk is aan “/” 
>>```
>>HTTP/1.0 200 OK↵ 
>>Content-type: text/html↵ 
>>↵ 
>>Dit is de eerste pagina. <a href="/pagina2">Ga naar pagina 2</a> 
>>```
>>Test wederom ook in je eigen browser om te kijken of deze pagina’s het doen. 
>>
>>#### c. HTTP file server 
>>Maak een uitbreiding op onderdeel b) zodat de bestandsnaam nu wordt opgezocht in een directory op je harde schijf. Indien het bestand bestaat, moet dit bestand naar de client gestuurd worden. Indien het bestand niet bestaat, moet de volgende data teruggegeven worden: 
>>```
>>HTTP/1.0 404 Not Found↵ 
>>Content-type: text/html↵ 
>>↵ 
>><h1>Dit bestand kon niet gevonden worden</h1> 
>>```
