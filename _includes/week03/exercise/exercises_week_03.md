>>> ### C# Programmeren – Opgaven week 3
>>> Auteur: Paul de Mast, Etiënne Goossens, Hans van der Linden
>>> Versie: 1
>>> Datum: 15-09-2020
>>>
>>> De leerdoelen van deze les zijn:
>>>-	Delegates
>>>-	Netwerkcommunicatie
>>>-	Client/Server in C# (met TcpClient)
>>>
>>> ### Oefening C# 3.1 delegates
>>> Test het gegeven delegate voorbeeld en maak een eigen variant.
>>>- Definieer een eigen class en een delegate die door die class wordt gebruikt
>>>- Creëer buiten de class twee methoden die je als delegate aan de class meegeeft.
>>>
>>> ### Oefening C# 3.2 client / server
>>> Test het gegeven Client / Server voorbeeld. Test de volgende situaties
>>>- Verschillende coderingen: tekst, byte buffer
>>>- Meerdere clients
>>>- Hoe kan gedetecteerd worden dat een verbinding is verbroken?
>>>- Wat gebeurt er als de laatste regel geen regelovergang bevat (zoals bij regelgebaseerde protocollen)?
>>>- Wanneer kun je de methode `StreamReader.ReadToEnd()` gebruiken? 
>>>- Wat gebeurt er bij `buffer overflow` (meer dan 256 bytes)?
>>>
>>> ### Oefening C# 3.3 robuuster maken en length prefixing
>>> Pas het programma aan zodat de server laat zien van welke client de verbinding komt
>>> Maak de applicatie robuuster zodat je o.a. een verbroken verbinding kunt ontdekken. Bedenk een geschikte oplossing voor message framing met behulp van length prefixen. Voor voorbeelden van implementaties zie:
>>>- Simple Message Framing Sample for TCP Socket: https://blogs.msdn.microsoft.com/joncole/2006/03/20/simple-message-framing-sample-for-tcp-socket/
>>>- TCP/IP .NET Sockets FAQ: https://blog.stephencleary.com/2009/04/tcpip-net-sockets-faq.html
>>>
>>> ### Opgave 3: miniproject (keuze uit 2 projecten)
>>> Kies uit de twee projecten op Blackboard er eentje uit en werk die in C# uit:
>>> 1.	Maak een eenvoudige HTTP server
>>> 2.  Client / Server opzet voor spellen waarbij de timing van het antwoord een rol speelt
>>>
>>> Volgende week ga je een GUI hiervoor bouwen.
>{: .exercise}
