# Gebruiksaanwijzing

### opladen / vervangen batterijen
De batterijen steekt u in de bijhorende batterijhouders met de juiste polariteiten. Als de batterij(en) minder dan 3V hebben, moeten ze opgeladen worden in de bijhorende oplader. Als u de batterijen te ver ontlaadt, moeten ze vervangen worden.

### draadloze communicatie
#### verbinding maken
Als u de aan/uit schakelaar bedient, zal u de lijnvolger aanzetten (ook de bluetooth module, herkenbaar met een snel pinklicht). Als u dan met een seriële bluetooth monitor app op uw gsm verbind met de bluetooth module, zal er de boodschap opkomen "connected" in de terminal en zal het lichtje zeer traag pinken met een groot interval

#### commando's
debug [on/off]:
Met dit commando kan u zien wat u ervoor heeft ingesteld van de onderstaande parameter + de waarden van de leessensor en de calculation time.

start :
Als u dit verzend in de terminal, zal de lijnvolger beginnen rijden

stop:
Als u dit verzend in de terminal, zal de lijnvolger met onmiddelijke ingang stoppen

set cycle [µs]:
Hiermee kunnen we zeggen hoelang er minimaal mag aan gewerkt worden aan 1 procedure

set power [0..255]:
De snelheid waarmee de lijnvolger mag rijden wordt gezegd door deze parameter. hoe hoger de parameter, hoe sneller het rijdt.

set diff [0..1]:
De nauwkeurigheid, voor de lijn te volgen in de bocht, wordt met deze parameter bepaald, hoe hoger de parameter hoe laxer hij omgaat met de curve van de lijn in de bocht.

set kp [0..]  :
Met dit kunnen we de lijnvolger zeggen dat die bij een grote fout sterk mag bijsturen bij een grote kp waarde, en bij een kleine kp waarde een klein beetje mag bijsturen. Deze parameter gaat ook de sterkte van de bochtsturing bepalen, volgt hij niet goed zijn bocht mag kp een hogere waarde hebben.

set ki [0..]:
Met deze parameter gaan de lijnvolger kijken hoe lang de fout zich blijft voordoen bij een afwijking. Hoe langer de fout zich voordoet, hoe sterker de lijnvolger gaat bijregelen. Een hogere waarde gaat de lijnvolger nog rapper bijregelen dan ervoor

set kd [0..]:
Hier gaat de lijnvolger kijken hoe snel de fout veranderd is tegenover de vorige cyclus. Is het verschil met de fout uit de vorige cyclus groot, dan gaan we sterk bijsturen. Is het verschil eerder klein dan sturen we minder sterk bij.

calibrate black:  
We leren de lijnvolger wat het kleur "zwart" is.

calibrate white:
We leren de lijnvolger wat het kleur "wit" is.

### kalibratie
Met de commandos "calibrate black" en "calibrate white" leren we de lijnvolger het verschil kennen tussen zwart en wit. Als de lijnvolger dan de lijn moet volgen, zal hij onmiddelijk zien door de zwarte kleur waar de lijn is.

### settings
De robot rijdt stabiel met volgende parameters: 
cycle time 10,
power 120,
kp 17,
ki 0.20,
kd 0.55,
diff 0.05

### start/stop button
uitleg locatie + werking start/stop button
