# Handreiking Wmebv e-formulieren en notificaties

- [Handreiking Wmebv e-formulieren en notificaties](#handreiking-wmebv-e-formulieren-en-notificaties)
  - [Introductie](#introductie)
    - [Totstandkoming handreiking](#totstandkoming-handreiking)
    - [Doel van deze handreiking](#doel-van-deze-handreiking)
    - [Doelgroep](#doelgroep)
    - [Samenwerkingspartners](#samenwerkingspartners)
  - [Wet Modernisering Bestuurlijk Verkeer](#wet-modernisering-bestuurlijk-verkeer)
    - [Wmebv samengevat in vier punten](#wmebv-samengevat-in-vier-punten)
    - [Wat zijn 'Formele berichten'?](#wat-zijn-formele-berichten)
    - [Wmebv schematisch weergegeven](#wmebv-schematisch-weergegeven)
  - [Project: e-formulieren en notificaties in het licht van de Wmebv](#project-e-formulieren-en-notificaties-in-het-licht-van-de-wmebv)
    - [Ontwerpcriteria voor E-formulieren en Notificaties](#ontwerpcriteria-voor-e-formulieren-en-notificaties)
      - [Best Practices](#best-practices)
        - [Gebruiksvriendelijke Identificatieprocessen](#gebruiksvriendelijke-identificatieprocessen)
        - [Periodieke Evaluatie en Bijwerking](#periodieke-evaluatie-en-bijwerking)
      - [Praktische adviezen voor het toetsen van e-formulieren en notificaties](#praktische-adviezen-voor-het-toetsen-van-e-formulieren-en-notificaties)
    - [Praktische Toepassing: Onze Aanpak in de praktijk](#praktische-toepassing-onze-aanpak-in-de-praktijk)
      - [Project Achtergrond en Doelstelling](#project-achtergrond-en-doelstelling)
      - [Wat is NL Design System](#wat-is-nl-design-system)
      - [Hoe gebruik je NL Design System als ontwerper en developer?](#hoe-gebruik-je-nl-design-system-als-ontwerper-en-developer)
      - [Het ontwerp van het generieke formulier in Figma](#het-ontwerp-van-het-generieke-formulier-in-figma)
      - [Development en Code Snippets (Verwijzing)](#development-en-code-snippets-verwijzing)
      - [Usability Tests en Resultaten](#usability-tests-en-resultaten)
  - [Geleerde Lessen en Aanbevelingen](#geleerde-lessen-en-aanbevelingen)
  - [Aanvullende Bronnen en Links voor Verdieping](#aanvullende-bronnen-en-links-voor-verdieping)
    - [Links](#links)
    - [Stappenplan implementatie Wmebv](#stappenplan-implementatie-wmebv)
    - [Overige interessante bronnen](#overige-interessante-bronnen)

## Introductie

### Totstandkoming handreiking

Deze handreiking is tot stand gekomen in opdracht van de Vereniging van Nederlandse Gemeenten Realisatie (VNGR) in samenwerking met NL Design System. Voor de handreiking zijn verschillende bronnen gebruikt. Naast desk-research is er een generiek e-formulier op basis van het NL Design System ontworpen en ontwikkeld. Het generieke e-formulier en de bijbehorende scenario's zijn ontwikkeld om inzage te geven in hoe enerzijds omgegaan zou kunnen worden met producten die nog niet beschikken over een e-formulier en anderzijds om te laten zien hoe met het gebruik van NL Design System binnen een relatief korte tijd gekomen kan worden tot een gebruikersvriendelijk en toegankelijk e-formulier. Het e-formulier en de bijbehorende vervolgschermen, en daarmee dus het scenario, zijn voorgelegd aan experts binnen de VNG, de NL Design System Community en tevens getoetst door Stichting Accessibility zodat deze handreiking in de praktijk gevalideerd is.

### Doel van deze handreiking

De doel van deze handreiking is om inzichten te delen betreft het ontwerpen en ontwikkelen van een generiek e-formulier op basis van NL Design System zodat deze voldoet aan de wet modernisering bestuurlijk verkeer (Wmebv). Tevens wordt gekeken naar wat de Wmebv betekent voor notificaties. De volgende onderwerpen worden in deze handreiking behandeld:

- Wmebv in het kort
- Ontwerpcriteria voor het maken van Wmebv proof e-formulieren en notificaties
- Het ontwerpen en ontwikkelen van een generiek formulier met behulp van NL Design System voor een brede generieke inzet.
- Implementatieadviezen met betrekking tot het Wmebv proof maken van e-formulieren en notificaties.

### Doelgroep

Deze handreiking is bestemd voor ieder die meer te weten wil komen over het Wmebv proof maken van e-formulieren en notificaties.

### Samenwerkingspartners

Deze handreiking en de bijbehorende schermvoorbeelden zijn een samenwerking van VNGR met het NL Design System kernteam, (UX) designers uit de NL Design System Community en met name de UX designer van Gemeente Den Haag, waar al veel onderzoek gedaan is naar de gebruikersvriendelijkheid van notificaties.

## Wet Modernisering Bestuurlijk Verkeer

In de Handreiking van Het Ministerie van Binnenlandse Zaken in samenwerking met Logius wordt het doel van deze wet helder benoemd:

> "De regering wil in het kader van de digitaal werkende overheid komen tot de implementatie van het wetsvoorstel modernisering elektronisch bestuurlijk verkeer. Met name de huidige regel dat een bestuursorgaan verkeer via de elektronische weg moet toestaan en dus ook kan uitsluiten, wordt als verouderd ervaren. Kabinetsbeleid is daarom dat bedrijven en burgers zaken die ze met de overheid doen – zoals het aanvragen van een vergunning – digitaal moeten kunnen afhandelen. Elektronisch bestuurlijk verkeer kan bijdragen aan de vermindering van administratieve lasten van burgers en bestuurlijke lasten van bestuursorganen. De wet neemt belemmeringen weg en stelt enkele randvoorwaarden aan de modernisering en digitalisering van de werkprocessen binnen de publieke sector. Burgers en bedrijven krijgen het recht (niet de plicht) om ieder formeel bericht elektronisch aan de overheid te zenden. Bij gebruik van de elektronische weg gelden er nieuwe waarborgen, waardoor nog meer rechtsbescherming wordt gerealiseerd. Tegelijkertijd houden bestuursorganen ruimte om digitale processen af te stemmen op de eigen organisatie. Om een compacte, efficiënte overheid te realiseren met hoogwaardige dienstverlening, is digitalisering een vereiste en is het digitale kanaal het voorkeurskanaal. Het uitgangspunt is: digitaal waar het kan. Het doel van de Wmebv is om regels over elektronisch bestuurlijk verkeer te moderniseren en burgers en bedrijven het recht te geven om elektronisch zaken te doen met de overheid. Degenen die dat willen moeten voor het digitale kanaal kunnen kiezen in hun contact met de overheid. Om te waarborgen dat iedereen met de overheid kan (blijven) communiceren, is het van belang dat communicatie langs de papieren weg mogelijk blijft. En dat de provincie een inclusief beleid voor ondersteuning van bepaalde doelgroepen gaat uitvoeren."

Bron: [Handreiking implementatie Wet modernisering elektronisch bestuurlijk verkeer (Awb) 2023.](https://www.digitaleoverheid.nl/wp-content/uploads/sites/8/2017/04/Handreiking-implementatie-Wet-modernisering-elektronisch-bestuurlijk-verkeer-2023.pdf)

### Wmebv samengevat in vier punten

De Wmebv is een belangrijk element in de bredere digitale transformatie van overheidsdiensten in Nederland en het is ontworpen om de overgang naar een meer digitaal georiënteerd bestuurlijk verkeer te vergemakkelijken.

- Wmebv is een wijziging van de Algemene Wet Bestuursrecht
- Wmebv geeft het recht op digitaal communiceren met bestuursorganen
- Wmebv stelt het openstellen van digitale kanalen verplicht, voor ieder formeel bestuurlijk bericht gericht aan het bestuursorgaan
- Wmebv resulteert in het aanpassen van digitale kanalen zodat het aan de wettelijk gestelde eisen voldoet.

### Wat zijn 'Formele berichten'?

Voordat er iets dieper ingegaan wordt over de Wmebv, is het belangrijk om aan te geven om wat voor berichtenverkeer het gaat in de Wmebv. In de diverse documentatie betreft de Wmebv wordt er op verschillende manieren gerefereerd naar het 'Elektronisch Bestuurlijk Verkeer''. Dit verkeer, in de vorm van digitale berichten, wordt in diverse documentatie ook wel 'Officiële berichten', 'Formele berichten' en 'Formeel officiële berichten' genoemd. In alle gevallen wordt hetzelfde bedoeld. In deze handreiking wordt de term 'formele berichten' aangehouden. Met het Elektronische Bestuurlijk Verkeer worden dus de 'formele berichten' bedoeld en deze verwijzen doorgaans naar officiële communicatie tussen verschillende bestuurlijke niveaus binnen een overheid. Deze berichten bevatten vaak belangrijke mededelingen, beslissingen, of andere informatie van juridische of bestuurlijke aard. Enkele veelvoorkomende voorbeelden:

- Berichten die deel uit maken van een procedure of besluit (zoals bijvoorbeeld: een aanvraag, zienswijze, ingebrekestelling of bezwaarschrift)
- een klacht
- anders krachtens wettelijk voorschrift voorgeschreven bericht. Bijvoorbeeld een melding.

Niet-officieel bestuurlijke berichten zijn alle andere berichten zoals informele contacten.

Het exacte bereik en de aard van formele berichten kunnen sterk variëren, dus het is belangrijk om de specifieke wetgeving en bestuurlijke structuren in overweging te nemen om een vollediger beeld te krijgen van welke producten onder deze term vallen. Voor deze handreiking is het echter van belang het verschil tussen niet formele berichten en formele berichten aan te duiden, om zo duidelijk te maken dat de Wmebv niet voor alle processen/producten geldt maar enkel voor de formele berichten. Voor meer verdieping in de juridische aspecten wordt verwezen naar de video-opname van [Kennissessie 1:  Juridisch Aspecten](https://youtu.be/7Vujk18JA-g) van 9 oktober 2023, die te vinden is op de website: [VNG webinars en kennissessies](https://vng.nl/wmebv-webinars-en-kennissessies)

### Wmebv schematisch weergegeven

Om toch in deze handreiking een idee te geven van de strekking van de Wmebv, wat veel verder strekt dan enkel e-formulieren en notificaties, worden de belangrijkste aspecten op een rij gezet.
Zie echter voor een zeer uitgebreide toelichting op de Wmebv de [Handreiking implementatie Wet modernisering elektronisch bestuurlijk verkeer (Awb) 2023.](https://www.digitaleoverheid.nl/wp-content/uploads/sites/8/2017/04/Handreiking-implementatie-Wet-modernisering-elektronisch-bestuurlijk-verkeer-2023.pdf) van het Ministerie van Binnenlandse Zaken.

Allereerst is het belangrijk om te weten dat de Wmebv over processen of beter gezegd, communicatiestromen gaat. Communicatiestromen tussen burger en overheidsinstantie. De stroom van een formeel bericht kent een begin en een eind. De stroom verloopt in verschillende fasen. Een formeel bericht wordt geïnitieerd (Zie het schema: 'Voor ontvangst') en vervolgens verstuurd. Als het goed gaat, wordt het bericht ontvangen door de overheidsinstantie (Zie het schema: 'Na ontvangst'). Vervolgens wordt het bericht in behandeling genomen en tijdens de behandeling kunnen vervolgacties voor de burger of instantie voortvloeien. Deze acties worden uitgevoerd, gelogd en er wordt over gecommuniceerd (zie het schema: 'Uitgaande formele berichten'), net zolang tot de behandeling van de initiële vraag of de daaruit voortgevloeide vragen of acties afgehandeld zijn. Naast de ze digitale communicatiestroom van formele berichten tussen burger en instantie, regelt de Wmebv een zorgplicht die stelt dat er voor passende ondersteuning gezorgd moet worden voor de mensen die minder goed mee kunnen komen in de digitale wereld.

![Wmebv-schema.png](.media/img_7.png)

De aspecten van de Wmebv zijn op te delen in onder andere een aantal blokken met daarin fasen waarin een formeel bericht zich bevindt:

**Blok 1 - Binnenkomende formele berichten:**
Dit blok is onder te verdelen in twee fasen:

**Fase 1 - Voor ontvangst:**\
Een formeel bericht kan op verschillende manieren binnenkomen, afhankelijk van het gekozen/aangeboden digitale kanaal. Denk aan:

- Een generiek contactformulier met upload mogelijkheid. (Later in deze handreiking wordt een voorbeeld behandeld van een generiek formulier.)
- E-mailkanaal (Echter, de meningen zijn nog verdeeld over hoe veilig dit medium is.)
- Specifiek webformulier met DigiD / e-Herkenning
- Via een MijnOmgeving
- Via een Berichtenbox (Bijvoorbeeld MijnOverheid)

De Wmebv regelt dat instanties de wijze van indienen bekend maken door kanalen aan te wijzen en dit bijvoorbeeld vast te leggen in een aanwijzingsbesluit en de burgers te informeren over het aangewezen digitale kanaal.
Er zijn een aantal belangrijke punten voordat een officieel bericht ontvangen kan worden:

- De digitale weg veilig moet veilig zijn. Belastende of onveilige berichten worden geweigerd.
- Er mogen geen technische eisen gesteld worden die onnodig belemmerend zijn.
- Er mogen geen gegevens afgedwongen worden zonder grondslag. Alleen noodzakelijke gegevens mogen worden uitgevraagd.
- De gemeente heeft de bevoegdheid tot het verlengen van de indieningstermijn bij storing en dient dit bekend te maken op bijvoorbeeld de website.

**Fase 2 - Na ontvangst:**\
De Wmebv regelt dat er ontvangstbevestiging verstuurd moet worden. Indien berichten intern doorgeleid zijn of afgewezen zijn, dient dit medegedeeld te worden.

Intern doorgeleiden is verplicht als:

- het bericht zonder nadere bewerking behandeld kan worden
- het bezwaarschrift of beroepsschrift is
- voor het type bericht geen wijze van verzending is aangewezen.
- de aanvang wettelijke behandeltermijn opschuift naar tijdstip van het intern doorleiden
- mededelingen aan de afzender van het doorgeleiden en tijdstip waarop de termijn aanvangt

De Wmebv regelt ook dat indien een bericht verkeerd is ingezonden, en om die reden is afgewezen, dat er een mededeling aan de afzender gezonden moet worden waarin vermeld wordt wat de juiste wijze van indiening is.

De Wmebv regelt dat ingevulde gegevens van een e-formulier terug-getoond moeten worden. Hetzij via:

- een download mogelijkheid tijdens het aanvraagproces
- inzage via een MijnOmgeving
- het toezenden van het afschrift

**_Ontwerp-tip: Denk bij het ontwerpen van deze communicatie aan de hierboven genoemde punten._**

 Tot slot dient de gemeente bewijslast te hebben, dat betekent dat een systeem moet zijn waarin gegevens gelogd worden.

**Blok 2 - Uitgaande formele berichten:**\
Dit blok is niet verder onderverdeeld in fasen. Bij dit blok geld dat de Wmebv regelt dat als er genotificeerd wordt, dat er met een aantal zaken rekening gehouden moeten worden, namelijk:

- de afzender moet worden vermeld
- de aard van het bericht moet worden vermeld (Bijv. ontvangstbevestiging, beschikking, betalingsverplichting etc.)
- en een reactietermijn
- Indien een bericht of notificatie niet bezorgd kan worden (een bounce) dan moet het minimaal eenmaal opnieuw verzonden worden.
- De gemeente heeft een inspanningsverplichting om het juiste e-mailadres te achterhalen
- Notificaties moeten op andere wijze verzonden kunnen worden

**_Ontwerp-tip: Denk bij het ontwerpen van deze communicatie aan de hierboven genoemde punten._**

De gemeente heeft tevens een bewijslast en moet het volgende kunnen bewijzen:

- Het tijdstip van verzending of ontvangst
- De verzending met de samenhangende ontvangstbevestiging of notificatie
- Tijdstip inlog geadresseerde om kennis te nemen van een aan hem gezonden bericht
- Ontvangen meldingen van formele berichten die niet konden worden bezorgd

**Blok 3 - Zorgplicht:**\
Tot slot staat  in het schema de zorgplicht genoemd.
De Wmebv regelt tevens een zorgplicht voor passende ondersteuning bij communicatie.
Denk hierbij aan:

- Passende ondersteuning is afgestemd op de doelgroepen en hun vaardigheden (lezen, schrijven, omgaan met digitale apparaten)
- Passende ondersteuning is generiek (zoals informatie op een website) en persoonlijk (zoals hulp aan de telefoon of balie)
- Bij Passende ondersteuning is maatwerk niet verplicht
- Beleid over passende ondersteuning opstellen en publiceren op de website (bijvoorbeeld regels of een (uiteraard toegankelijke) handreiking)

## Project: e-formulieren en notificaties in het licht van de Wmebv

In dit deel van de handreiking wordt toegelicht hoe er in samenwerking met NL Design System een generiek e-formulier is ontworpen, gebouwd en getest. Voorafgaand aan de bouw heeft deskresearch plaatsgevonden om ontwerpcriteria te verzamelen, niet alleen algemene ontwerpcriteria maar ook criteria die voortvloeien uit de Wmebv.

### Ontwerpcriteria voor E-formulieren en Notificaties

Hieronder een praktische lijst met ontwerpcriteria waarmee rekening gehouden dient te worden tijdens het ontwerp van e-formulieren en notificaties.

**Algemene ontwerpcriteria:**

(Let op, de \*\* gemarkeerde punten zijn ook van toepassing op de Wmebv.)

1. Vul invulvelden waar mogelijk voor in
2. Geef voorwaarden, uitleg, benodigde informatie, documenten aan
3. Gebruik duidelijke taal en begrippen
4. Licht vragen en termen toe, waar nodig
5. Vraag alleen noodzakelijke gegevens en informatie \*\*
6. Geef aan welke vragen/velden verplicht zijn
7. Geef foutmeldingen duidelijk en gebruikersvriendelijk aan
8. Geef processtap in formulier aan tijdens het invulproces
9. Ondersteun de bezoeker bij het invullen en afronden, door duidelijke knoppen
10. Zorg voor tussentijdse opslag van informatie

AVG-regeltjes waar rekening mee moet worden gehouden:

- Wees transparant
- Verzamel zo min mogelijk persoonsgegevens \*\*
- Vraag toestemming
- Gebruik eenvoudige taal
- Verzend e-formulieren over versleutelde verbindingen. \*\*
- Registreer verwerking in verwerkingsregister \*\*

**Wmebv ontwerpcriteria:**
Op zich zijn onderstaande punten niet perse e-formulier ontwerpcriteria, echter moet er wel rekening mee gehouden worden tijdens het ontwerp van de communicatiestroom waar het e-formulier of notificatie onderdeel vanuit maakt.

- Toon of verstuur (indien mogelijk) een ontvangstbevestiging
- Maak ingevulde gegevens toegankelijk voor de indiener.

Deze lijst is onder andere geput uit de door de VNG aangeboden [Toolkit Meten en Verbeteren van Webformulieren.](https://vng.nl/kennisbank-dienstverlening-gemeenten/toolkit-meten-en-verbeteren-van-webformulieren)

> Bied een gedetailleerd overzicht van de specifieke eisen van de Wmebv die van toepassing zijn op e-formulieren en notificaties.
> Koppel deze eisen aan specifieke elementen in het generieke formulierontwerp en leg uit hoe deze worden ingevuld.
> (Inzoom op e-forms Wmebv)

#### Best Practices

##### Gebruiksvriendelijke Identificatieprocessen

Besteed aandacht aan de gebruiksvriendelijkheid van het identificatieproces. Zorg ervoor dat gebruikersinterventies intuïtief zijn en dat de stappen helder zijn gepresenteerd. Minimaliseer de kans op fouten en voorzie duidelijke instructies.

##### Periodieke Evaluatie en Bijwerking

Identificatie- en authenticatiemethoden evolueren voortdurend. Het is raadzaam om periodiek de gebruikte methoden te evalueren en, indien nodig, bij te werken om te blijven voldoen aan de laatste standaarden en beveiligingseisen.

#### Praktische adviezen voor het toetsen van e-formulieren en notificaties

Bij het toetsen van formulieren en notificaties in het kader van de Wet modernisering elektronisch bestuurlijk verkeer (Wmebv) is het van belang om te zorgen dat deze voldoen aan de eisen van de wet, met een focus op digitale toegankelijkheid en gebruiksvriendelijkheid. Hier zijn enkele specifieke punten waaraan je aandacht zou moeten besteden:

1. Digitale Toegankelijkheid
Zorg ervoor dat formulieren en notificaties voldoen aan de richtlijnen voor digitale toegankelijkheid, zoals vastgesteld in de Web Content Accessibility Guidelines (WCAG). Hierbij gaat het onder andere om het gebruik van leesbare tekst, voldoende contrast, en de mogelijkheid om het formulier met toetsenbord te bedienen.

2. Gebruiksvriendelijkheid (Usability)
Test de formulieren en notificaties op algemene gebruiksvriendelijkheid. Zijn ze intuïtief en gemakkelijk te begrijpen voor de gebruiker? Zorg ervoor dat de taal eenvoudig en duidelijk is, en dat gebruikers gemakkelijk door het formulier of de notificatie kunnen navigeren.

3. Rechtsgeldigheid en Authenticatie
Controleer of de gebruikte elektronische handtekeningen en authenticatiemethoden voldoen aan de wettelijke vereisten voor rechtsgeldigheid. Zorg ervoor dat er passende maatregelen zijn genomen om de identiteit van de gebruiker te verifiëren.

4. Privacybescherming
Wees alert op privacykwesties bij het verzamelen en verwerken van persoonsgegevens. Zorg ervoor dat de formulieren en notificaties voldoen aan de Algemene Verordening Gegevensbescherming (AVG) en andere relevante privacywetgeving.

5. Veiligheid
Controleer of er voldoende beveiligingsmaatregelen zijn genomen, met name bij het verzenden van gevoelige informatie. Beveiligde verbindingen (HTTPS) en versleuteling van gegevens zijn hierbij belangrijk.

6. Aanpasbaarheid en Responsiviteit
Zorg ervoor dat formulieren en notificaties goed werken op verschillende apparaten en schermformaten. Responsiviteit is essentieel voor een goede gebruikerservaring op zowel desktops als mobiele apparaten.

7. Duidelijke Instructies en Hulpfuncties
Bied duidelijke instructies bij het invullen van formulieren en zorg voor eventuele hulpfuncties indien nodig. Gebruikers moeten gemakkelijk de benodigde informatie kunnen vinden en begrijpen hoe ze het formulier moeten invullen.

8. Notificatie-Inhoud en Timing
Bij notificaties is het belangrijk dat de inhoud relevant, begrijpelijk en tijdig is. Vermijd overbodige informatie en zorg ervoor dat de notificatie op het juiste moment wordt verstuurd.

9. Testen met Gebruikers
Voer usability-tests uit met echte gebruikers om inzicht te krijgen in hun ervaring en eventuele pijnpunten te identificeren. Dit kan helpen bij het verbeteren van de algehele gebruikerservaring.

10. Naleving van Wmebv-specifieke Eisen
Controleer of de formulieren en notificaties specifieke eisen van de Wmebv naleven.

### Praktische Toepassing: Onze Aanpak in de praktijk

#### Project Achtergrond en Doelstelling

Om een praktisch voorbeeld te kunnen geven van een generiek e-formulier is er samengewerkt met NL Design System om binnen een relatief korte tijd te komen tot een generiek voorbeeld formulier dat inzage verschaft in het ontwerpproces en de bouw met behulp van NL Design System componenten. Er is gekozen voor een generiek formulier, omdat dit het meest laagdrempelige formulier is wat wellicht initieel ingezet kan worden, met name voor die processen die nog niet over een (specifiek) formulier beschikken.

Om de use case van dit generieke formulier te ondersteunen is nagedacht over een scenario waarin dit formulier gebruikt zou kunnen worden. Om het scenario aan te laten sluiten bij op de Wmebv, is in overleg met een jurist gekomen tot een situatie waarbij de fictieve burger (Persona: Jeroen van Drouwen) de gemeente waarin hij woonachtig is (Gemeente Voorbeeld) in gebreken te stellen.

**Het scenario:**

- Scenario flow

#### Wat is NL Design System

- Algemeen verhaal NLDS
  
#### Hoe gebruik je NL Design System als ontwerper en developer?

NL Design componenten met een eigen huisstijl.
Korte beschrijving waarom/het nut Design Token en de samenwerking dev en designer en voor meer info hier:
[NL Design Tokens](https://www.nldesignsystem.nl/meedoen/design-tokens/)

#### Het ontwerp van het generieke formulier in Figma

- Hoe tot stand gekomen?
  - Community van ontwerpers Forms Forms Forms, Design Open Hour
  - geleerd van andere onderzoeken
- Al het geleerde en mbv de NLDS library schermen bouwen
- schematische flows scenario
- Voorbeeldschermen Gemeente voorbeeld

[Gemeente Voorbeeld Live demo](https://www.gemeentevoorbeeld.nl/wmebv)

#### Development en Code Snippets (Verwijzing)

(To come op NL Design System website)

#### Usability Tests en Resultaten

(To come na de usability tests)

## Geleerde Lessen en Aanbevelingen

- uitkomsten usability tests
- maak gebruik van de community, vraag feedback (Design Open Hour)
- test altijd het ontwerp!

## Aanvullende Bronnen en Links voor Verdieping

### Links

- ...
- ...

### Stappenplan implementatie Wmebv

Voor meer informatie over een mogelijke aanpak voor de implementatie van de Wmebv wordt verwezen naar dit [Stappenplan](https://vng.nl/artikelen/stappenplan-wet-mebv) ter ondersteuning bij de implementatie van de Wmebv binnen uw organisatie, waarin de volgende onderwerpen behandeld worden:

**Digitalisering van de dienstverlening:**

1. Wat vraagt de Wmebv?
2. Hoe kan ik het aanpakken?
3. Slim digitaliseren met de [omnichannelaanpak](https://vng.nl/omnichannel).
4. Analyse huidige digitale kanalen met behulp van de [Uniforme Productnamen Lijst](https://vng.nl/projecten/uniforme-productnamen-lijst-upl)
5. Besluit en communiceer de gekozen kanalen.
6. Bepaal uw beleid t.a.v. een ([Omnichannel](https://vng.nl/omnichannel)) kanaalstrategie.
7. Aan de gang met implementeren.

**Zorgplicht bij de dienstverlening:**

1. Bepaal welke belemmeringen inwoners ervaren
2. Bepaal hoe u belemmeringen kunt wegnemen.
3. Leg uw keuzes voor zorgplicht vast in een beleidsdocument.
4. Communiceer hoe uw gemeente ondersteunt bij de dienstverlening.

### Overige interessante bronnen

- links
  