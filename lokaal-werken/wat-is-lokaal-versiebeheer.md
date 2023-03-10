# Wat is lokaal versiebeheer?

{% hint style="success" %}
[Kennisclip](https://ap.cloud.panopto.eu/Panopto/Pages/Viewer.aspx?id=07633b1b-ded1-479d-ba4a-ad8d00b8242e)
{% endhint %}

## Inleiding

Als je nog nooit met versiebeheer gewerkt hebt, kan het moeilijk zijn om je een goed beeld te vormen van hoe alle puzzelstukjes van Git in elkaar passen. Laat ons het dus eerst even hebben over wat Git precies is, voor we het leren gebruiken.

Git is een **systeem voor versiebeheer**, dat wil zeggen een systeem om oudere versies van je project op een ordelijke manier bij te houden. Als je geen oude versies bijhoudt, riskeer je belangrijke code te verliezen (bv. als je in een nieuwe versie een kritieke bug vindt die er in een oude versie niet was). Je kan klassieke backups maken door regelmatig al je code te zippen, maar voor je het weet, heb je enorm veel schijfruimte verbruikt of weet je niet meer in welk bestand de interessantste aanpassingen gebeurd zijn. Met een goed systeem voor versiebeheer gaat dat soort werk veel efficiënter.

Meestal bestaat dat project dat je met een versiebeheersysteem beheert uit code, maar dat hoeft niet. Je kan er vanalles mee bijhouden, van tekeningen in Illustrator tot recepten. Zelfs data in die je niet kan voorstellen als leesbare tekst is mogelijk, bijvoorbeeld audiobestanden, maar versiebeheersystemen komen het best tot hun recht als de data in een tekstformaat staat.

We zullen hier een voorbeeld geven van **lokaal gebruik** van Git. Dat wil zeggen dat we op één machine aan versiebeheer doen. Git is ook enorm populair voor teams, maar we beginnen bij het begin.

## Rodedraadvoorbeeld

{% hint style="info" %}
Bij onderstaand voorbeeld wordt een tekening gemaakt in de kennisclip.
{% endhint %}

### stap 1: onvoorzichtige aanpak

Nabil is een programmeur die een complex programma aan het schrijven is. Laat ons zeggen, een online boodschappenlijstje met HTML, CSS en JavaScript. Hij/zij werkt een drie maanden aan dit boodschappenlijstje. Maand 1 zorgt hij dat je items kan toevoegen, Maand 2 dat je items kan aanduiden als "gekocht", maand 3 voor de layout.

Voor Nabil naar huis gaat, stuurt hij aan het einde van maand 3 zijn code naar de manager en die is tevreden van de functionaliteit, maar vindt de layout maar niets.

Nu moet Nabil terug naar de versie van het einde van maand 2. Alle code voor de layout verwijderen kost veel werk. Achteraf bekeken was het beter geweest om regelmatig een backup te maken. We bekijken even hoe dit er had uitgezien.

### stap 2: regelmatige backups

Zelfde scenario. Aan het einde van elke dag maakt Nabil een backup van alle files in een zipbestand met naam DAG-MAAND-JAAR. Voor Nabil naar huis gaat, stuurt hij aan het einde van maand 3 zijn code naar de manager en die is tevreden van de functionaliteit, maar vindt de layout maar niets. Op de eerste dag van maand september pakt Nabil er de code van 31 juli bij, begint hij aan een nieuwe layout.

De backups helpen wel, maar zijn op zich niet genoeg.

### stap 3: backups met metadata

Nabil zou makkelijk terug kunnen gaan naar de gewenste code als hij de tijdlijn had bijgehouden die je in dit filmpje ziet. Hij zou een tekstbestand of spreadsheet kunnen bijhouden met de wijzigingen op elk moment. Waar op de vorige tijdlijn steeds een backup werd aangegeven, moet je je nu inbeelden dat we een spreadsheet aanvullen met de datum van vandaag.

### stap 4: simpel versiebeheersysteem

De vorige aanpak dat is erg lastig om up-to-date te houden, zeker omdat je in de praktijk soms meerdere backups per uur zou moeten nemen om niets kwijt te raken. Dus Nabil schrijft een ander programma om bij deze taak te helpen. Dit programma kan eenvoudig backup nemen van de huidige toestand van de versie van de code en er een beschrijving van opslaan.

Dit tweede programma is een heel eenvoudig versiebeheersysteem. Het maakt het veel makkelijker oude code bij te houden en te onthouden wat op welk moment is gebeurd. Een versiebeheersysteem zoals Git biedt in essentie deze zelfde voordelen en meer, maar pakt de zaken nog veel efficiënter aan dan hoe wij het hier hebben geschetst. Voorlopig is het voldoende als je weet dat je met een versiebeheersysteem een tijdlijn van je code kan maken zoals je die hier hebt gezien.

## demonstratie echte Git commando's

In de kennisclip bij deze pagina wordt een demonstratie gegeven van hoe dit er allemaal uitziet in de praktijk. **Je hoeft de commando's niet te onthouden. Sterker, probeer de commando's meteen na dit filmpje te vergeten, want je past ze best pas toe als je de details beter begrijpt.** Die leggen we verder in de cursus één voor één uit. Hier moet je gewoon luisteren naar de uitleg.

## Mogelijkheden van versiebeheer

Enkele dingen die zonder versiebeheer heel lastig zijn en met versiebeheer erg eenvoudig worden:

* een logboek met allerlei versies van je code bijhouden
* je code delen met collega’s (met heel duidelijk afgebakende momentopnames en zonder risico dat ze jouw code overschrijven, in tegenstelling tot een gedeelde OneDrive of Dropbox)
* de verschillen tussen twee specifieke versies van je code bekijken
* experimenteren met twee oplossingen voor één probleem, zodat je achteraf de beste oplossing kan kiezen
