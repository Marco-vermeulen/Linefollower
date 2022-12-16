# Instructable

Een instructable is een stappenplan - zonder verdere uitleg - hoe je vertrekkend van de bill of materials en gebruik makend van de technische tekeningen de robot kan nabouwen. Ook de nodige stappen om de microcontroller te compileren en te uploaden staan beschreven.  

### stap 1
bestel alle componenten uit de bill of materials 

### stap 2
Wacht tot alle componenten zijn toegekomen

### stap 3
Soldeer de componenten waar nodig. (motoren met kabels, leessensor met pinnen, Aan/uit schakelaar met + draad batterij en kabel, motor driver met pinnen)

### stap 4
Maak de chassis uit een MDF-houtplaat volgens de mechanische tekening.

### stap 5
bevestig de arduino mega op het MDF-houtplaatje met schroeven

### stap 6
Bevestig het breadbord op de USB-poort en batterijpoort van de arduino met de kleefband

### stap 7
bevestig de aan/uit schakelaar aan de korte zijkant naar keuze met lijm

### stap 8
zet de drukknop, led,  motor driver en bluetooth module in het breadbord en sluit aan volgens het elektronisch schema. Zet de batterijhouders in het midden tussen de pinnen op de arduino.

### stap 9
Bevestig de leessensor met ducktape aan de voorkant van de chassis, en sluit aan volgens het elektronisch schema.

### stap 10
Bevestig de motoren zo ver mogelijk aan de achterzijde onder de chassis met lijm. Sluit daarna aan volgens het elektronisch schema. verleng de draden met een extra draad waar nodig.

### stap 11
zet de wielen op beide assen van de motoren, plak eventueel een stukje ductape over de kabels als die over de grond zouden slepen.

### stap 12
de lijnvolger zou nu moeten geconstrueerd zijn volgens de foto. Als dit het geval is, gaan we over naar het programmeren.

### stap 13
Download de code met de bijhorende bibliotheken, en open de (.ino) bestand in arduino IDE

### stap 14
(ALS OP LIJN 1 EN 2 staat "#include "SerialCommand.h"" EN "#include "EEPROMAnything.h"", SLA DE VOLGENDE STAPPEN OVER EN GA NAAR STAP 16) Importeer de bijhorende bibliotheken via schets-> bibliotheek gebruiken -> .ZIP bibliotheek toevoegen. Selecteer dan in de file explorer op "all files" en importeer alle bestanden die ghedownloadded zijn (behalve de .INO file!)

### stap 15
Ga dan opnieuw naar schets-> bibliotheek gebruiken, in de lijst zou nu de geïmporteerde bibliotheken staan op hun namen zelf of onder de bestands naam. Klik op de bibliotheken in kwestie. de lijnen "#include "SerialCommand.h"" en "#include "EEPROMAnything.h"" zouden in het begin erbij komen

### stap 16
Klik op het vinkje links boven in het IDE venster. Als er geen errors komen in het zwart venster beneden het IDE venster, sluit dan de Arduino aan uw computer (belangrijk: batterij voeding mag NOOIT aangeschakeld worden als u de arduino aansluit op uw computer, schakel om met de AAN/UIT  schakelaar indien nodig!).

### stap 17
Ga dan naar Hulmpiddelen -> Board -> Arduino AVR boards -> Arduino Mega or Mega 2560. Check ook als de processor goed is bij de tab hulpmiddelen. Het is namelijk een ATMega2560. Selecteer dan ook de bijhorende COM-poort in de tab Hulpmiddelen

### stap 18
Klik daarna op het pijltje, naast het vinkje, links boven in het IDE venster. Als het gelukt is, zou de boodschap "uploadden voltooid" verschijnen boven het zwart venster.

### stap 19
Ontkoppel de Arduino. Zet de AAN/UIT schakelaar aan, verbind uw smartphone met de lijnvolger volgens de stappen in de gebruiksaanwijzing.

### stap 20
Calibreer de sensor volgens de gebruiksaanwijzing

### stap 21
Voer daarna de settings in volgens de bijhorende commando's beschreven in de gebruiksaanwijzing.

### stap 22
Start de lijnvolger met de bijhorende commando in de gebruiksaanwijzing

### stap 23
Monitor't het gedrag van de lijnvolger, als de lijnvolger effectief doet zoals het hoort ga naar stap 25. Als de lijnvolger niet doet zoals  het hoort. Stop de lijnvolger met het bijhorend commando in de gebruiksaanwijzing en ga naar stap 24.

### stap 24
Pas de settings aan waar nodig en ga daarna terug naar stap 22

### stap 25
proficiat! u heeft een werkende lijnvolger! Als het gewenst is, kan u nog de settings aanpassen als u de lijnvolger nog sneller en efficiënter wilt laten gaan. in dat geval ga naar stap 24.

