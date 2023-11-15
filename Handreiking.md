

- [1. Inleiding](#1-inleiding)
  - [1.1. Totstandkoming handreiking](#11-totstandkoming-handreiking)
  - [1.2. Doel van deze handreiking](#12-doel-van-deze-handreiking)
  - [1.3. Samenwerkingspartners](#13-samenwerkingspartners)
- [2. Achtergrond Wmebv](#2-achtergrond-wmebv)
  - [2.1. Wmebv in het kort](#21-wmebv-in-het-kort)
    - [2.1.1 Doel van Wmebv](#211-doel-van-wmebv)
    - [2.1.2 Belangrijkste aspecten van de Wmebv](#212-belangrijkste-aspecten-van-de-wmebv)
    - [2.1.3 Samengevat in vier punten](#213-samengevat-in-vier-punten)
  - [2.2. Formeel Bestuurlijke berichten](#22-formeel-bestuurlijke-berichten)
- [3. Relevante Wmebv-vereisten voor e-formulieren en notificaties](#3-relevante-wmebv-vereisten-voor-e-formulieren-en-notificaties)
    - [3.0.1. Identificatie en Authenticatie](#301-identificatie-en-authenticatie)
      - [3.0.1.1. Uitleg over de Wmebv-vereisten](#3011-uitleg-over-de-wmebv-vereisten)
    - [3.0.2. Implementatiestrategieën](#302-implementatiestrategieën)
      - [3.0.2.1. Gestructureerde Identificatieprocessen](#3021-gestructureerde-identificatieprocessen)
      - [3.0.2.2. Encryptie en Beveiligde Communicatie](#3022-encryptie-en-beveiligde-communicatie)
    - [3.0.3. Best Practices](#303-best-practices)
      - [3.0.3.1. Gebruiksvriendelijke Identificatieprocessen](#3031-gebruiksvriendelijke-identificatieprocessen)
      - [3.0.3.2. Periodieke Evaluatie en Bijwerking](#3032-periodieke-evaluatie-en-bijwerking)
    - [3.0.4. Praktische adviezen voor het toetsen van e-formulieren en notificaties](#304-praktische-adviezen-voor-het-toetsen-van-e-formulieren-en-notificaties)
- [4. Toegankelijkheid](#4-toegankelijkheid)
  - [4.1. Digitale Toegankelijkheid](#41-digitale-toegankelijkheid)
    - [4.1.1. ARIA-labels en Schermlezers](#411-aria-labels-en-schermlezers)
      - [4.1.1.1. Praktische Gids voor het Gebruik van ARIA-labels](#4111-praktische-gids-voor-het-gebruik-van-aria-labels)
    - [4.1.2. Demonstratie van Schermlezer-vriendelijke Ontwerpen](#412-demonstratie-van-schermlezer-vriendelijke-ontwerpen)
  - [4.2. Contrast en Leesbaarheid](#42-contrast-en-leesbaarheid)
    - [4.2.1. Diepgaande Analyse van Contrastverhoudingen en Lettergroottes](#421-diepgaande-analyse-van-contrastverhoudingen-en-lettergroottes)
    - [4.2.2. Richtlijnen voor het Verbeteren van Leesbaarheid](#422-richtlijnen-voor-het-verbeteren-van-leesbaarheid)
  - [4.3. Logische Navigatie](#43-logische-navigatie)
    - [4.3.1. Voorbeelden van Logische Navigatiestructuren](#431-voorbeelden-van-logische-navigatiestructuren)
    - [4.3.2. Implementatietips voor een Intuïtieve Gebruikerservaring](#432-implementatietips-voor-een-intuïtieve-gebruikerservaring)
- [5. Generiek Formulier](#5-generiek-formulier)
  - [5.1. Desk-research e-forms/notificeren (non-Wmebv)](#51-desk-research-e-formsnotificeren-non-wmebv)
  - [5.2. Wat is een Design System](#52-wat-is-een-design-system)
    - [5.2.1. NL Design System](#521-nl-design-system)
    - [5.2.2. Hoe werkt NL Design Systems](#522-hoe-werkt-nl-design-systems)
      - [5.2.2.1. De opbouw van het NL Design System](#5221-de-opbouw-van-het-nl-design-system)
    - [5.2.3. Design van Generiek e-formulier op basis van NLDS](#523-design-van-generiek-e-formulier-op-basis-van-nlds)
    - [5.2.4. Development van generieke e-formulier op basis van NLDS](#524-development-van-generieke-e-formulier-op-basis-van-nlds)
    - [5.2.5. Toegankelijkheidstesten door Stichting Accessibility van het ontwikkelde e-formulier](#525-toegankelijkheidstesten-door-stichting-accessibility-van-het-ontwikkelde-e-formulier)
- [6. Implementatieadvies e-formulieren en notificaties](#6-implementatieadvies-e-formulieren-en-notificaties)
  - [6.1. Indicatief Stappenplan voor het Wmebv-proof maken van producten](#61-indicatief-stappenplan-voor-het-wmebv-proof-maken-van-producten)
  - [6.2. Praktische adviezen voor de implementatie van formulieren en notificaties](#62-praktische-adviezen-voor-de-implementatie-van-formulieren-en-notificaties)
- [7. Onderhoud en Evolutie:](#7-onderhoud-en-evolutie)
- [8. Contact en Ondersteuning:](#8-contact-en-ondersteuning)
- [9. Conclusie:](#9-conclusie)


## 1. Inleiding

### 1.1. Totstandkoming handreiking
Deze handreiking is tot stand gekomen in opdracht van de Vereniging van Nederlandse Gemeenten Realisatie (VNGR) in samenwerking met NL Design System. Voor de handreiking zijn verschillende bronnen gebruikt. Naast desk-research is er een generiek e-formulier op basis van het NL Design System ontworpen en ontwikkeld. Het generieke e-formulier en de bijbehorende scenario's zijn ontwikkeld om inzage te geven in hoe enerzijds omgegaan zou kunnen worden met producten die nog niet beschikken over een e-formulier en anderzijds om te laten zien hoe met het gebruik van NL Design System binnen een relatief korte tijd gekomen kan worden tot een gebruikersvriendelijk en toegankelijk e-formulier. Het e-formulier en de bijbehorende vervolgschermen, en daarmee dus het scenario, zijn voorgelegd aan experts binnen de VNG, de NL Design System Community en tevens getoetst door Stichting Accessibility zodat deze handreiking in de praktijk gevalideerd is. 

### 1.2. Doel van deze handreiking
Het is van groot belang dat digitale toegankelijkheid en gebruikersvriendelijkheid gewaarborgd wordt en in overeenstemming is met de Wmebv.
Daarom wordt in deze handreiking meegedacht over:
- Ontwerpcriteria voor het maken van Wmebv proof e-formulieren en notificaties
- Het ontwerpen en ontwikkelen van een generiek formulier met behulp van NL Design System voor een brede generieke inzet.
- Implementatieadviezen met betrekking tot het Wmebv proof maken van e-formulieren en notificaties.

### 1.3. Samenwerkingspartners 
Deze handreiking en de bijbehorende schermvoorbeelden zijn een samenwerking van VNGR met het NL Design System kernteam, (UX) designers uit de NL Design System Community en met name de UX designer van Gemeente Den Haag, waar al veel onderzoek gedaan is naar de gebruikersvriendelijkheid van notificaties. 

## 2. Achtergrond Wmebv

### 2.1. Wmebv in het kort  
De Wet digitale overheid (WDO), waarvan de volledige titel Wet modernisering elektronisch bestuurlijk verkeer (Wmebv) is, is een Nederlandse wet die tot doel heeft het digitale verkeer tussen de overheid en burgers, bedrijven en instellingen te moderniseren en te verbeteren. 

#### 2.1.1 Doel van Wmebv  
Voor een heldere toelichting wordt verwezen naar bron: [Handreiking implementatie Wet modernisering elektronisch bestuurlijk verkeer (Awb) 2023.][def].
>**Digitaal zaken doen met de overheid.  **  
De regering wil in het kader van de digitaal werkende overheid komen tot de implementatie van het wetsvoorstel modernisering elektronisch bestuurlijk verkeer. Met name de huidige regel dat een bestuursorgaan verkeer via de elektronische weg moet toestaan en dus ook kan uitsluiten, wordt als verouderd ervaren. Kabinetsbeleid is daarom dat bedrijven en burgers zaken die ze met de overheid doen – zoals het aanvragen van een vergunning – digitaal moeten kunnen afhandelen. Elektronisch bestuurlijk verkeer kan bijdragen aan de vermindering van administratieve lasten van burgers en bestuurlijke lasten van bestuursorganen. De wet neemt belemmeringen weg en stelt enkele randvoorwaarden aan de modernisering en digitalisering van de werkprocessen binnen de publieke sector. Burgers en bedrijven krijgen het recht (niet de plicht) om ieder formeel bericht elektronisch aan de overheid te zenden. Bij gebruik van de elektronische weg gelden er nieuwe waarborgen, waardoor nog meer rechtsbescherming wordt gerealiseerd. Tegelijkertijd houden bestuursorganen ruimte om digitale processen af te stemmen op de eigen organisatie. Om een compacte, efficiënte overheid te realiseren met hoogwaardige dienstverlening, is digitalisering een vereiste en is het digitale kanaal het voorkeurskanaal. Het uitgangspunt is: digitaal waar het kan. Het doel van de Wmebv is om regels over elektronisch bestuurlijk verkeer te moderniseren en burgers en bedrijven het recht te geven om elektronisch zaken te doen met de overheid. Degenen die dat willen moeten voor het digitale kanaal kunnen kiezen in hun contact met de overheid. Om te waarborgen dat iedereen met de overheid kan (blijven) communiceren, is het van belang dat communicatie langs de papieren weg mogelijk blijft. En dat de provincie een inclusief beleid voor ondersteuning van bepaalde doelgroepen gaat uitvoeren. 

#### 2.1.2 Belangrijkste aspecten van de Wmebv
De aspecten van de Wmebv zijn op te delen in onder andere een aantal fasen waarin een formeel bericht zich bevind:
- Fase: Voor ontvangst
  - De Wmebv regelt dat Formele berichten digitaal ontvangen kunnen worden. Dat kan op verschillende manieren voorzien worden:
    -  Een generiek contactformulier met upload mogelijkheid (Later in deze handreiking wordt een voorbeeld gedeeld.)
    -  E-mail kanaal (maar daar zijn de meningen over verdeeld...)
    -  Specifiek webformulier met DigiD / e-Herkenning
    -  Via een MijnOmgeving
    -  Via een Berichtenbox (Bijvoorbeeld MijnOverheid)
  - De Wmebv regelt dat instanties de wijze van indienen bekend maken door kanalen aan te wijzen en dit bijvoorbeeld vast te leggen in een aanwijzingsbesluit. En de burgers te informeren over het aangewezen digitale kanaal.
  - het is in tevens van belang dat de digitale weg veilig is. Daarbij mogen Belastende of onveilige berichten worden geweigerd.
  - Ook mogen er geen technische eisen gesteld worden die onnodig belemmerend zijn
  - Er mogen geen gegevens afgedwongen worden zonder grondslag. Alleen noodzakelijke gegevens mogen worden uitgevraagd.
  - Tot slot heeft de gemeente de bevoegdheid tot het verlengen van de indieningstermijn bij storing en dient dit bekend te maken op bijvoorbeeld de website.

- Fase: Na ontvangst
  - De Wmebv regelt dat er ontvangstbevestiging verstuurd moet worden. Indien berichten intern doorgeleid zijn of afgewezen zijn, dient dit medegedeeld te worden.
  - Intern doorgeleiden is verplicht als:
    - Het bericht zonder nadere bewerking behandeld kan worden 
    - Het bezwaarschrift of beroepsschrift is
    - Voor het type bericht geen wijze van verzending is aangewezen
    - Aanvang wettelijke behandeltermijn opschuift naar tijdstip van het intern doorleiden
    - Mededelingen aan de afzender van het doorgeleiden en tijdstip waarop de termijn aanvangt
  - De Wmebv regelt ook dat indien een bericht verkeerd is ingezonden, en om die reden is afgewezen, dat er een mededeling aan de afzender gezonden moet worden waarin vermeld wordt wat de juiste wijze is.
  - De Wmebv regelt dat ingevulde gegevens van een e-formulier terug-getoond moeten worden. Hetzij via:
    -  een download mogelijkheid tijdens het aanvraagproces
    -  inzage via een MijnOmgeving
    -  het toezenden van het afschrift
 -  Tot slot dient de gemeente bewijslast te hebben, dat betekent dat een systeem moet zijn waarin gegevens gelogd worden.

- Fase: Uitgaand
  - De Wmebv regelt dat als er genotificeerd wordt, dat er een aantal zaken aangeduid moeten worden:
    -  de afzender
    -  de aard van het bericht (Bijv. ontvangstbevestiging, beschikking, betalingsverplichting etc.)
    -  en een reactietermijn
 -  Indien een bericht of notificatie niet bezorgd kan worden (een bounce) dan moet het minimaal eenmaal opnieuw verzonden worden.
 -  De gemeente heeft een inspanningsverplichting om het juiste e-mailadres te achterhalen
 -  Notificaties moeten op andere wijze verzonden kunnen worden
 -  De gemeente heeft tevens een bewijslast en moet het volgende kunnen bewijzen:
    -  Het tijdstip van verzending of ontvangst
    -  De verzending met de samenhangende ontvangstbevestiging of notificatie
    -  Tijdstop inlog geaddersseerde om kennis te nemen van een aan hem gezonden bericht
    -  Ontvangen meldingen van formele berichten die niet konden worden bezorgd
  
- Zorgplicht
  - De Wmebv regelt tevens een zorgplicht voor passende ondersteuning bij communicatie.
  - Passende ondersteuning:
    - Afgestemd op de doelgroepen en hun vaardigheden (lezen, schrijven, omgaan met digitale apparaten)
    - Ondersteuning is generiek (zoals informatie op een website) en persoonlijk (Zoals hulp aan de telefoon of balie)
    - Maatwerk is niet verplicht
    - Beleid opstellen en publiceren op de website (bijvoorbeeld regels of een handreiking)
  - Hoe inkaderen
    - Wat is de visie op dienstverlening?
    - Data over klantgedrag samenbrengen
    - Begrijpen wat de belemmeringen zijn
    - Beleid maken op passende ondersteuning


![picture 0](images/b3672d2338f7bc0115d4bd0ce64b06fe0b986619097a70ea609c5279be4c6185.png)  



De Wmebv is een belangrijk element in de bredere digitale transformatie van overheidsdiensten in Nederland, en het is ontworpen om de overgang naar een meer digitaal georiënteerd bestuurlijk verkeer te vergemakkelijken.

#### 2.1.3 Samengevat in vier punten  
- Wmebv is een wijziging van de Algemene wet Bestuursrecht
- Wmebv geeft het recht op digitaal communiceren met bestuursorganen
- Wmebv stelt het openstellen van digitale kanalen verplicht, voor ieder formeel bestuurlijk bericht gericht aan het bestuursorgaan
- Wmebv resulteert in het aanpassen van digitale kanalen zodat het aan de wettelijk gestelde eisen voldoet.

Zie voor een zeer uitgebreide toelichting op de Wmebv: [Handreiking implementatie Wet modernisering elektronisch bestuurlijk verkeer (Awb) 2023.][def]

### 2.2. Formeel Bestuurlijke berichten
'Formeel Bestuurlijke berichten' verwijzen doorgaans naar officiële communicatie tussen verschillende bestuurlijke niveaus binnen een overheid. Deze berichten bevatten vaak belangrijke mededelingen, beslissingen, of andere informatie van juridische of bestuurlijke aard. De precieze aard van Formeel Bestuurlijke berichten kan variëren afhankelijk van de wetgeving en bestuurlijke structuren in een specifieke jurisdictie, maar hier zijn enkele veelvoorkomende voorbeelden:
- Beschikking
- Bekendmaking
- Kennisgeving

Enkele voorbeelden:  

1. Besluiten van het College van B&W:  
Mededelingen van besluiten die zijn genomen door het College van Burgemeester en Wethouders binnen een gemeente. Dit kan bijvoorbeeld betrekking hebben op vergunningen, beleidsveranderingen of andere belangrijke lokale aangelegenheden.

2. Provinciale Verordeningen:  
Berichten met betrekking tot verordeningen of besluiten van het provinciebestuur. Deze kunnen van invloed zijn op alle gemeenten binnen een provincie.

3. Rijksbesluiten:  
Officiële communicatie van de centrale overheid naar lagere bestuursniveaus, zoals provincies en gemeenten. Dit kan bijvoorbeeld betrekking hebben op wijzigingen in nationale wetgeving.

4. Juridische Aankondigingen:  
Bekendmakingen van juridische aard, zoals rechterlijke uitspraken, die relevant zijn voor het bestuurlijke proces.

5. Beleidsmededelingen:  
Communicatie over wijzigingen in beleid op verschillende bestuursniveaus. Dit kan variëren van lokaal tot nationaal beleid.

6. Aankondigingen van Publieke Raadplegingen:  
Berichten die aankondigen dat er publieke raadplegingen of inspraakprocedures zullen plaatsvinden met betrekking tot voorgesteld beleid of projecten.

7. Informatie over Verkiezingen:  
Aankondigingen met betrekking tot verkiezingen, stemprocedures en resultaten op verschillende bestuursniveaus.

8. Financiële Aankondigingen:  
Mededelingen over financiële zaken, zoals begrotingen, subsidies, belastingtarieven en andere financiële aangelegenheden.

Het exacte bereik en de aard van Formeel Bestuurlijke berichten kunnen sterk variëren, dus het is belangrijk om de specifieke wetgeving en bestuurlijke structuren in overweging te nemen om een vollediger beeld te krijgen van welke producten onder deze term vallen.


> TODO: Geef een overzicht van de Wet en benadruk de relevante secties met betrekking tot e-formulieren en notificaties.
>(Diagram Hendrik) + verwijzingen naar BZK_Deloitte
(big picture Wmebv - klantreis) (Figma voorbeeld getoetst met Juliette van der Jagt en op basis van Service Blue print Vincent van Beek)

## 3. Relevante Wmebv-vereisten voor e-formulieren en notificaties

> Bied een gedetailleerd overzicht van de specifieke eisen van de Wmebv die van toepassing zijn op e-formulieren en notificaties.
Koppel deze eisen aan specifieke elementen in het generieke formulierontwerp en leg uit hoe deze worden ingevuld.
(Inzoom op e-forms Wmebv)

#### 3.0.1. Identificatie en Authenticatie

##### 3.0.1.1. Uitleg over de Wmebv-vereisten
De Wet modernisering elektronisch bestuurlijk verkeer (Wmebv) stelt specifieke eisen aan het proces van identificatie en authenticatie bij elektronische formulieren en notificaties. Het doel van deze eisen is om de veiligheid en betrouwbaarheid van interacties tussen burgers en overheidsinstanties te waarborgen. In lijn met de Wmebv moeten identificatie en authenticatie zodanig worden vormgegeven dat ze de wederzijdse erkenning van digitale identiteiten mogelijk maken, met specifieke aandacht voor privacy en beveiliging.

#### 3.0.2. Implementatiestrategieën

##### 3.0.2.1. Gestructureerde Identificatieprocessen
Om te voldoen aan de Wmebv is het van belang gestructureerde identificatieprocessen te implementeren. Dit omvat het gebruik van erkende identificatiemiddelen, zoals DigiD, eHerkenning, of andere goedgekeurde digitale identiteitsoplossingen. Het identificatieproces moet duidelijk en transparant zijn voor de gebruiker, waarbij de keuze voor het identificatiemiddel op een begrijpelijke wijze wordt gepresenteerd.

##### 3.0.2.2. Encryptie en Beveiligde Communicatie
Een cruciaal aspect van identificatie en authenticatie is de beveiliging van de communicatie tussen gebruikers en de overheid. Door gebruik te maken van end-to-end-encryptie en beveiligde protocollen wordt gewaarborgd dat persoonlijke gegevens veilig worden uitgewisseld. Dit voldoet niet alleen aan de Wmebv, maar draagt ook bij aan de bescherming van de privacy van de gebruiker. 
>(BRON??)

#### 3.0.3. Best Practices

##### 3.0.3.1. Gebruiksvriendelijke Identificatieprocessen
Besteed aandacht aan de gebruiksvriendelijkheid van het identificatieproces. Zorg ervoor dat gebruikersinterventies intuïtief zijn en dat de stappen helder zijn gepresenteerd. Minimaliseer de kans op fouten en voorzie duidelijke instructies.

##### 3.0.3.2. Periodieke Evaluatie en Bijwerking
Identificatie- en authenticatiemethoden evolueren voortdurend. Het is raadzaam om periodiek de gebruikte methoden te evalueren en, indien nodig, bij te werken om te blijven voldoen aan de laatste standaarden en beveiligingseisen.

#### 3.0.4. Praktische adviezen voor het toetsen van e-formulieren en notificaties
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
Denk hier bij aan de volgende punten:
    - Vraag geen onnodige informatie
    - Toon of verstuur (indien mogelijk) een ontvangstbevestiging
    - Maak ingevulde gegevens toegankelijk voor de indiener.

>>>> * TODO Zijn formulieren slim te combineren?
>>>> * TODO Contactformulier voorzien van een stapje ervoor, waaruit de aard van het contact naar voren komt, zodat deze op het "juiste spoor" gezet kan worden. Met juiste spoor kan bepaald worden of het gaat om een bericht met een rechtsgevolg (en dus valt onder Wmebv) en welke niet. Voor meer juridische informatie verwijzen we u graag naar (iets van Juliette? Juridische pagina VNG - Wmebv? )
![Voorbeeld van vooraf categoriseren](https://hackmd.io/_uploads/H1yvdr3eT.png) (Dit plaatje in NLDS stijl maken...)
>>>> * adviezen over labeling (refereren aan Form Form Form) "Indienen" of "Uploaden"
>>>> * (OVER TAAL)Uit onderzoeken blijkt duidelijke overheidcommunicatie niet duidelijk https://vng.nl/projecten/duidelijke-overheidscommunicatie

>---------TODO---------------
>* (Wmebv CRITERIA - NOG TE VERWERKEN van Jurist) Als je het hebt over berichten waarvoor je een notificatie wilt regelen, ga ik ervan uit dat je alleen kijkt naar het kanaal “systeem voor gegevensverwerking waarin de geadresseerde toegang heeft tot het bericht”.  (Voor andere kanalen geldt de notificatieplicht namelijk niet). Aan het gebruik van dit kanaal zelf stelt de Wmebv ook eisen, maar ik beperk me tot de eisen die t.a.v. specifiek notificatie relevant zijn. Het gaat om de volgende eisen:

>    * De notificatie moet binnen 48 uur na plaatsing van het bericht in het systeem voor gegevensverwerking aan de geadresseerde van het bericht worden gestuurd

>    * De notificatie moet het bericht ontsluiten (bijv. als de notificatie per app wordt gestuurd) OF

>   * De notificatie moet de volgende informatie bevatten:
    1. welk bestuursorgaan heeft het bericht in het systeem van gegevensverwerking geplaatst,
    2. de aard en rechtsgevolgen van het bericht (bijv. is het een ontvangstbevestiging, een beschikking, een betalingsverplichting, een uitnodiging voor het geven van een zienswijze of een uitnodiging voor een hoorzitting; en wat betekent dit bericht voor de burger.)
    3. indien van toepassing, de termijn waarbinnen de geadresseerde kan of moet reageren (bijv. termijn waarbinnen bezwaar kan worden gemaakt tegen een besluit, een betaling moet zijn verricht, of stukken kunnen worden ingediend). 

 

   > * Als de notificatie niet met succes bij de geadresseerde kan worden bezorgd, moet de kennisgeving nog een keer worden verzonden of moet de gemeente op een andere manier contact zoeken met de geadresseerde om hem te laten weten dat de notificatie niet kan worden bezorgd.
    * Toelichting: Het hangt af van de soort bounce welke actie de gemeente moet nemen: bij een soft bounce (een tijdelijk probleem bij het afleveren van de notificatie) doordat de mailbox van de geadresseerde vol is of zijn mailserver tijdelijk niet bereikbaar is of het bericht te groot is, kan de gemeente de notificatiemail nog een keer sturen.
    Bij een hard bounce (het mailadres bestaat niet of is ongeldig) waarbij de gemeente herhaaldelijk een melding krijgt dat een notificatie niet is ontvangen heeft nog een keer verzenden van de notificatie geen zin. In dat geval moet de gemeente zich inspannen om de geadresseerde voor notificaties te bereiken (door geadresseerde per telefoon of brief erover te informeren dat de notificatie niet kan worden bezorgd en welke maatregelen hij kan nemen om notificaties te ontvangen)

   > * Indien de notificatie niet is verzonden of de burger deze niet heeft ontvangen, leidt dat ertoe dat een overschrijding van een termijn die is begonnen te lopen met de verzending van het bericht zelf hem niet kan worden tegengeworpen. Van een bestuursorgaan wordt dan verwacht dat hij bewijst, met een logverslag, dat de notificatie is verzonden en geen bericht is ontvangen dat de aflevering is mislukt. Als het bestuursorgaan kan aantonen dat de notificatie is verzonden, zo nodig een tweede keer als de eerste aflevering is mislukt, moet de geadresseerde aan te tonen dat deze niet is ontvangen en dat niet aan hem is te verwijten.

>**(NOG TE VERWERKEN) Wmebv criteria om rekening mee te houden tijdens het bouwen van e-forms**
>- lijstje punten + referenties -> zie lijst

>**(NOG TE VERWERKEN) Wmebv criteria om rekening mee te houden tijdens het bouwen van notificaties**
>- lijstje punten + referenties -> zie lijst  
(Hendrik - meeting Werkgroep harmonisatie berichtenverkeer)  
Bronvermelding + figma schetsen (o.b.v. Rozarin meldingen?)

-----------------------------
>>>> Deel best practices voor het ontwerpen en implementeren van e-formulieren in overeenstemming met de Wmebv.
Overweeg voorbeelden en casestudy's om de principes tastbaar te maken.
(NLDS Formulieren site, VNG Toolkit)

## 4. Toegankelijkheid

Het belang van toegankelijkheid bij e-formulieren en notificaties is van cruciaal belang voor het creëren van een inclusieve digitale omgeving. Toegankelijkheid verwijst naar het ontwerp en de ontwikkeling van digitale producten en diensten op een manier die ervoor zorgt dat alle gebruikers, inclusief mensen met verschillende capaciteiten en beperkingen, er effectief toegang toe hebben en deze kunnen gebruiken. Hier zijn enkele belangrijke redenen waarom toegankelijkheid bij e-formulieren en notificaties een prioriteit zou moeten zijn:

- Inclusiviteit en Gelijke Kansen  
Toegankelijke e-formulieren en notificaties zorgen ervoor dat alle burgers, ongeacht hun fysieke, cognitieve, sensorische of andere capaciteiten, gelijke toegang hebben tot de digitale diensten van de overheid. Dit draagt bij aan het principe van inclusiviteit en gelijke kansen voor iedereen.

- Wettelijke Vereisten  
In veel jurisdicties zijn er wettelijke vereisten met betrekking tot digitale toegankelijkheid. Door te voldoen aan deze wettelijke normen, zoals vastgesteld in richtlijnen zoals de Web Content Accessibility Guidelines (WCAG), kunnen organisaties juridische compliance waarborgen.

- Breder Publiek Bereiken  
Toegankelijke e-formulieren vergroten het bereik van de diensten naar een breder publiek. Het stelt mensen met diverse vaardigheden en behoeften in staat om deel te nemen aan het digitale proces, wat essentieel is voor een democratische samenleving.

- Verbetering van de Gebruikerservaring  
Toegankelijkheidsprincipes gaan vaak hand in hand met algemene verbeteringen in de gebruikerservaring. Het creëren van e-formulieren en notificaties die duidelijk, gestructureerd en gemakkelijk te begrijpen zijn, komt alle gebruikers ten goede.

- Beter Imago en Dienstverlening  
Het tonen van betrokkenheid bij digitale toegankelijkheid draagt bij aan het imago van de organisatie als een inclusieve en klantgerichte entiteit. Het versterkt het vertrouwen van burgers in de digitale dienstverlening van de overheid.

- Voorkomen van Uitsluiting  
Niet iedereen ervaart digitale diensten op dezelfde manier. Onvoldoende toegankelijke e-formulieren en notificaties kunnen leiden tot digitale uitsluiting van bepaalde groepen, wat in strijd is met het principe van gelijkheid en inclusiviteit.

- Toekomstbestendigheid
Het nemen van toegankelijkheid in overweging bij het ontwerpen van e-formulieren en notificaties zorgt voor toekomstbestendigheid. Het maakt het gemakkelijker om aanpassingen te doen in reactie op veranderende behoeften of nieuwe technologieën.

- Maatschappelijk Verantwoord Ondernemen  
Het integreren van toegankelijkheidsprincipes in digitale dienstverlening weerspiegelt een maatschappelijk verantwoord ondernemen. Het laat zien dat een organisatie zich inzet voor het welzijn van alle burgers.

Kortom, toegankelijkheid is niet alleen een ethische en wettelijke vereiste, maar het is ook een essentiële pijler voor het bouwen van inclusieve, effectieve en duurzame digitale diensten in de moderne samenleving.
Geef enkele voorbeelden van toegankelijkheidsverbeteringen die zijn doorgevoerd op basis van de testresultaten.

### 4.1. Digitale Toegankelijkheid

#### 4.1.1. ARIA-labels en Schermlezers

##### 4.1.1.1. Praktische Gids voor het Gebruik van ARIA-labels
Definitie en Doel van ARIA-labels: Accessible Rich Internet Applications (ARIA)-labels zijn hulpmiddelen om de toegankelijkheid van dynamische webcontent te verbeteren. Voor het implementeren van ARIA-labels is het essentieel om te begrijpen hoe ze effectief kunnen worden gebruikt om de gebruikerservaring te verbeteren.

Praktisch Voorbeeld:

```
<button aria-label="Sluit" onclick="sluitFormulier()">X</button>
```
Dit voorbeeld toont hoe een ARIA-label kan worden toegepast om de functie van een knop duidelijk te maken, waardoor schermlezers accurate informatie aan gebruikers kunnen verstrekken.

#### 4.1.2. Demonstratie van Schermlezer-vriendelijke Ontwerpen
Belang van Schermlezer-vriendelijk Ontwerp  
Een schermlezer vertaalt visuele informatie naar gesproken tekst, waardoor mensen met visuele beperkingen digitale content kunnen begrijpen. Het ontwerpen met schermlezers in gedachten verbetert de algemene toegankelijkheid van de website of applicatie.

Implementatietips  
Zorg voor informatieve en beknopte alt-tekst bij afbeeldingen.
Gebruik semantisch correcte HTML-tags voor een betere structurering van de content.
Vermijd uitsluitend op visuele elementen gebaseerde aanwijzingen.

### 4.2. Contrast en Leesbaarheid

#### 4.2.1. Diepgaande Analyse van Contrastverhoudingen en Lettergroottes
Belang van Contrast  
Een goede contrastverhouding tussen tekst en achtergrond is essentieel voor leesbaarheid, vooral voor mensen met verminderd zicht. De Web Content Accessibility Guidelines (WCAG) stellen specifieke eisen aan contrastverhoudingen.

Richtlijnen voor Verbetering  
Zorg voor een minimale contrastverhouding van 4.5:1 voor normale tekst en 3:1 voor grotere tekst (≥ 18pt of ≥ 14pt vet).
Gebruik een leesbaar lettertype met een voldoende grootte voor comfortabel lezen.

#### 4.2.2. Richtlijnen voor het Verbeteren van Leesbaarheid
Typografische Overwegingen  
Kies lettertypen met duidelijke, onderscheidende karakters.
Streef naar een regelafstand die voldoende ruimte biedt tussen tekstregels.

### 4.3. Logische Navigatie

#### 4.3.1. Voorbeelden van Logische Navigatiestructuren
Semantisch Correcte Navigatie  
Gebruik nav-elementen voor navigatieblokken.
Structureer links in lijsten voor betere semantiek.
Praktisch Voorbeeld:  

```
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#services">Services</a></li>
    <li><a href="#contact">Contact</a></li>
  </ul>
</nav>
```

#### 4.3.2. Implementatietips voor een Intuïtieve Gebruikerservaring
Gebruiksvriendelijke Navigatie   
Beperk het aantal navigatie-opties om keuzestress te voorkomen.
Geef duidelijke labels en beschrijvingen aan navigatie-elementen.

Verbetering van Focusnavigatie    
Zorg ervoor dat focusindicatoren duidelijk zichtbaar zijn.
Overweeg het gebruik van skip-links om direct naar belangrijke content te springen.

## 5. Generiek Formulier 

**Doel van het generieke formulier**
>Het doel voor het maken van een generiek formulier is...  
(Aanpak: Desk-research, ontwikkeling generiek voorbeeld forms, usability test)  
Introduceer het NL Design System en leg uit waarom het een waardevolle basis is voor e-formulieren.  
Beschrijf het generieke formulierontwerp en de schermflow die je hebt ontwikkeld, en leg uit hoe deze aansluiten bij de principes van het NL Design System.

### 5.1. Desk-research e-forms/notificeren (non-Wmebv)
>- Wat is er allemaal over e-forms onderzocht door VNG en anderen?
- Inzoomen op BZK-Deloitte bron Bijlage 3 over e-forms (Deze handreiking borduurt daarop verder)
- Onderzoeken Den Haag (bijv. * vs "optioneel", Rozarin etc)
- Best practices e-forms & notificeren, incl. hoe om te gaan met Taal (Verwijzing onderzoek BZK - Werkgroep Harmonisatie (Hendrik) )


### 5.2. Wat is een Design System
Een Design System is een gestructureerde verzameling van herbruikbare ontwerpelementen, -componenten en -richtlijnen die samenwerken om een consistente en coherente gebruikerservaring te creëren binnen een product of merk. Het is een centrale bron van waarheid voor het ontwerpteam en andere belanghebbenden, waarin essentiële ontwerpprincipes, visuele stijlen, interactiepatronen en codefragmenten worden gedocumenteerd.

In feite fungeert een Design System als een blauwdruk voor het bouwen en onderhouden van digitale producten. Het omvat vaak zowel het visuele ontwerp als de functionele aspecten van een applicatie, waardoor het niet alleen een hulpmiddel is voor ontwerpers, maar ook voor ontwikkelaars en andere teamleden die betrokken zijn bij het productieproces.

De voordelen van een Design System zijn talrijk. Het bevordert consistentie en efficiëntie in het ontwerpproces, omdat teams kunnen putten uit een gemeenschappelijke set van elementen in plaats van steeds opnieuw het wiel uit te vinden. Het verbetert de samenwerking tussen verschillende disciplines en vergemakkelijkt het onderhoud en de evolutie van producten na verloop van tijd.

Belangrijk is dat een Design System dynamisch is en kan evolueren met de behoeften van het product en het merk. Het is niet alleen een statische verzameling van ontwerpelementen, maar eerder een levend document dat wordt bijgewerkt naarmate het product groeit en verandert.

Kortom, een Design System is een waardevol instrument dat organisaties helpt bij het bouwen en onderhouden van samenhangende, gebruiksvriendelijke en schaalbare digitale producten en diensten.


#### 5.2.1. NL Design System
De Agenda Digitale Overheid stelt dat overheidsdienstverlening toegankelijk en begrijpelijk moet zijn voor iedereen. Hiervoor zijn consistent ontworpen diensten en websites nodig.

Om deze reden gaat de NL Design System (NLDS) overheidsorganisaties principes, interactiepatronen en code delen via een gezamenlijk design system. Dit NL Design System draagt niet alleen bij aan gebruiksvriendelijkere diensten van een betere kwaliteit en toegankelijkheid. Het helpt ook dubbel werk te voorkomen.

**Eén geteste toegankelijke huisstijl voor iedereen?**

In Nederland hebben de vele overheidsorganisaties een eigen identiteit en huisstijl. Rijkhuisstijl is voorbehouden voor de Rijksoverheid en mag door alle andere organisaties, zoals gemeentes, niet gebruikt worden. Dit is een belangrijk verschil met bijvoorbeeld GOV.UK, die wel één huisstijl kent die door lokale overheden gebruikt mag worden.

Met het NL Design System kan de hele overheid in Nederland samenwerken aan een begrijpelijke, gebruiksvriendelijke én toegankelijke online dienstverlening. Een dienstverlening die logisch en samenhangend is, maar niet per se uniform, want binnen de afspraken blijft er ruimte voor de eigen identiteit van overheidsorganisaties.

Door thema's te maken met beschikbare design tokens kunnen applicaties super snel gebruik maken van dezelfde componenten, zélfs als deze door een andere organisatie gebouwd zijn. Deze thema's kunnen dan weer goed getest worden op toegankelijkheid en gebruiksvriendelijkheid en voor de verschillende applicaties van een organisatie hergebruikt worden (zelfs als deze door verschillende leveranciers zijn gebouwd).

**Samen werken aan een herbruikbare componenten bibliotheek**
Het NL Design System bestaan uit een community van 430+ leden, een multidisciplinaire groep van geïnteresseerden van verschillende overheidsorganisaties en bedrijven die met overheden werken. Deze community heeft een gedeelde ambitie om niet telkens het wiel opnieuw uit te vinden, maar wil ook niet geblokkeerd worden in de ontwikkeling van nieuwe applicaties.

Kijk voor meer informatie over NL Design System op [de website van NLDS](https://nldesignsystem.nl/).

#### 5.2.2. Hoe werkt NL Design Systems

##### 5.2.2.1. De opbouw van het NL Design System
>(input presentatie Jeff over gelaagdheid en tokens enzo)

#### 5.2.3. Design van Generiek e-formulier op basis van NLDS
>(uitleg van aanpak/doel van de formulieren)

**Ontwikkeling Generiek e-form voorbeeld**
>Design Figma VNG obv NLDS     
(Generieke flow gemaakt & Goede vs slechte formulieren)  
(input voor UX designers bij gemeenten en leveranciers…)  
Screenshots

#### 5.2.4. Development van generieke e-formulier op basis van NLDS
>(input voor developers bij gemeenten en leveranciers…)  
Hoe werkt NLDS (input DS week talk Jeffrey over tokens enzo)  
Hoe is de ontwikkeling aangepakt?   
(Wat wil NLDS meegeven aan developers?)  
Link naar form(s)  

#### 5.2.5. Toegankelijkheidstesten door Stichting Accessibility van het ontwikkelde e-formulier
>  E-forms toetsen   
Hoe is het burgerpanel uitgevoerd?  
Usability  
Toegankelijkheidseisen  
Wmebv pointers  
(Input Rapport Accessibility)


## 6. Implementatieadvies e-formulieren en notificaties

> Bied praktisch advies voor gemeenten over hoe ze het generieke formulier in hun eigen systemen kunnen implementeren.
Verwijs naar relevante bronnen en ondersteunende documentatie.

### 6.1. Indicatief Stappenplan voor het Wmebv-proof maken van producten

ZIE: https://vng.nl/artikelen/stappenplan-wet-mebv

1. Inventariseer Producten:  
Begin met het inventariseren van alle producten en diensten die de gemeente aanbiedt. Maak hierbij gebruik van de [Uniforme Productlijst (UPL)](https://standaarden.overheid.nl/uplstandaarden.overheid.nl) om een volledig overzicht te krijgen.

1. Prioriteer op Basis van Digitale Interacties:  
Identificeer de producten en diensten die frequent digitale interacties vereisen, zoals aanvragen, meldingen, klachten, etc.

1. Digitale Toegankelijkheidsaudit:  
Voer een digitale toegankelijkheidsaudit uit voor de geselecteerde producten. Dit kan een evaluatie omvatten van bestaande formulieren, notificaties en digitale interacties.

1. Zaaksysteem Implementeren (indien mogelijk):  
Overweeg de implementatie van een zaaksysteem als een geïntegreerde oplossing voor het beheren van de levenscyclus van producten en diensten. Dit helpt bij het stroomlijnen van processen en het voldoen aan de eisen van de Wmebv.

1. Ontwerp Generieke E-Formulieren:  
Ontwerp generieke e-formulieren volgens de principes van het NL Design System. Zorg ervoor dat ze voldoen aan de eisen van de Wmebv en toegankelijk zijn voor alle gebruikers.

1. Implementeer Notificatiesysteem:  
Overweeg de implementatie van een notificatiesysteem om burgers op de hoogte te stellen van de status van hun aanvragen, meldingen, etc. Zorg ervoor dat notificaties begrijpelijk en toegankelijk zijn.

1. Toegankelijkheidstesten:  
Laat de ontwikkelde e-formulieren en notificaties testen op digitale toegankelijkheid door bijvoorbeeld Stichting Accessibility.

1. Training en Bewustwording:  
Train medewerkers in het gebruik van het zaaksysteem, e-formulieren en notificatiesysteem. Zorg voor bewustwording over digitale toegankelijkheid en de vereisten van de Wmebv.

1. Gebruikersfeedback Verzamelen:  
Verzamel gebruikersfeedback door middel van gebruikerstesten en feedbackformulieren. Pas het ontwerp en de functionaliteit aan op basis van deze input.

1.  Documenteer Procedures:  
Documenteer duidelijke procedures en richtlijnen voor het beheer en de update van e-formulieren, notificaties en andere digitale interacties.

1.  Continue Monitoring en Evaluatie:  
Zet een continue monitoring- en evaluatieproces op om ervoor te zorgen dat de digitale producten voldoen aan de eisen van de Wmebv en om aanpassingen te maken op basis van veranderende wetgeving of nieuwe inzichten.

1.  Kennisdeling:  
Faciliteer kennisdeling tussen gemeenten. Moedig gemeenten aan om ervaringen en best practices te delen om van elkaar te leren.


### 6.2. Praktische adviezen voor de implementatie van formulieren en notificaties
Praktisch advies voor de implementatie van het generieke formulier in de systemen van gemeenten kan zich richten op zowel technische als organisatorische aspecten. Hier zijn enkele specifieke adviezen:

1. Compatibiliteit met Bestaande Systemen:  
Zorg ervoor dat het generieke formulier compatibel is met de bestaande systemen van de gemeente. Dit kan integratie vereisen met CRM-systemen, databases en andere relevante platforms.

2. API-Integratie:  
Overweeg het gebruik van API's voor een soepele integratie. Goed gedocumenteerde API's vergemakkelijken de communicatie tussen het generieke formulier en andere systemen.

3. Gebruik van Standaarden:  
Houd rekening met geldende standaarden voor gegevensuitwisseling. Zorg ervoor dat het generieke formulier gegevens genereert en ontvangt volgens vastgestelde normen.

4. Beveiliging en Privacy:  
Besteed bijzondere aandacht aan beveiligingsaspecten. Zorg voor een versleutelde gegevensoverdracht en implementeer maatregelen om de privacy van burgers te waarborgen.

5. Training van Medewerkers:  
Train medewerkers die verantwoordelijk zijn voor het beheer van het generieke formulier. Zorg ervoor dat zij bekend zijn met het systeem, inclusief het aanpassen van formulieren en het interpreteren van ingevulde gegevens.

6. Monitoring en Onderhoud:
Implementeer monitoringtools om de prestaties van het generieke formulier te volgen. Stel een plan op voor regelmatig onderhoud, updates en bugfixes.

7. Schaalbaarheid Overwegen:  
Anticipeer op toekomstige groei en behoeften. Zorg ervoor dat het generieke formulier schaalbaar is en gemakkelijk kan worden aangepast aan veranderende vereisten.

8. Documentatie voor Implementatie:  
Zorg voor uitgebreide documentatie over de implementatie van het generieke formulier. Dit moet technische specificaties, configuratie-instructies en probleemoplossingsgidsen bevatten.

9. Ondersteuning van Leveranciers:  
Als het generieke formulier is ontwikkeld door een externe leverancier, zorg dan voor duidelijke afspraken over ondersteuning en onderhoud. Weet waar en hoe je ondersteuning kunt krijgen als dat nodig is.

10. Feedbackmechanismen Voorzien:  
Implementeer feedbackmechanismen voor zowel interne medewerkers als burgers. Dit helpt bij het identificeren van eventuele problemen en het verbeteren van de gebruikerservaring.

11. Testen in Realistische Omstandigheden:  
Voer uitgebreide tests uit in een omgeving die zo dicht mogelijk bij de productieomgeving ligt. Dit helpt bij het identificeren van mogelijke problemen voordat het generieke formulier in gebruik wordt genomen.

12. Verwijzing naar Relevante Bronnen:  
Bied links naar relevante bronnen en documentatie, inclusief handleidingen, tutorials en eventuele trainingen die beschikbaar zijn voor de gemeente.

Door deze praktische adviezen te volgen, kunnen gemeenten een soepele implementatie van het generieke formulier waarborgen, waardoor ze voldoen aan de eisen van de Wmebv en tegelijkertijd een effectieve en gebruiksvriendelijke digitale ervaring bieden aan hun burgers.


## 7. Onderhoud en Evolutie:

>Bespreek de noodzaak van voortdurend onderhoud en evolutie van e-formulieren in overeenstemming met de wetgeving en technologische ontwikkelingen.
Moedig gemeenten aan om regelmatig hun formulieren te evalueren en bij te werken.

## 8. Contact en Ondersteuning:

Heeft u vragen over de aanstaande wet? Benader dan het projectteam WMEBV: wmebv@vng.nl
Meer informatie is tevens te vinden op het [VNG Forum](https://forum.vng.nl/)

## 9. Conclusie:

>Sluit af met een samenvatting van de belangrijkste punten en moedig gemeenten aan om actie te ondernemen in de richting van toegankelijke en gebruiksvriendelijke e-formulieren.












[def]: https://www.digitaleoverheid.nl/wp-content/uploads/sites/8/2017/04/Handreiking-implementatie-Wet-modernisering-elektronisch-bestuurlijk-verkeer-2023.pdf