## 1 Introductie en Wmebv Overzicht
### 1.1. Totstandkoming handreiking

Deze handreiking is tot stand gekomen in opdracht van de Vereniging van Nederlandse Gemeenten Realisatie (VNGR) in samenwerking met NL Design System. Voor de handreiking zijn verschillende bronnen gebruikt. Naast desk-research is er een generiek e-formulier op basis van het NL Design System ontworpen en ontwikkeld. Het generieke e-formulier en de bijbehorende scenario's zijn ontwikkeld om inzage te geven in hoe enerzijds omgegaan zou kunnen worden met producten die nog niet beschikken over een e-formulier en anderzijds om te laten zien hoe met het gebruik van NL Design System binnen een relatief korte tijd gekomen kan worden tot een gebruikersvriendelijk en toegankelijk e-formulier. Het e-formulier en de bijbehorende vervolgschermen, en daarmee dus het scenario, zijn voorgelegd aan experts binnen de VNG, de NL Design System Community en tevens getoetst door Stichting Accessibility zodat deze handreiking in de praktijk gevalideerd is.

### 1.2. Doel van deze handreiking

Het is van groot belang dat digitale toegankelijkheid en gebruikersvriendelijkheid gewaarborgd wordt en in overeenstemming is met de Wmebv.
Daarom wordt in deze handreiking meegedacht over:

* Ontwerpcriteria voor het maken van Wmebv proof e-formulieren en notificaties
* Het ontwerpen en ontwikkelen van een generiek formulier met behulp van NL Design System voor een brede generieke inzet.
* Implementatieadviezen met betrekking tot het Wmebv proof maken van e-formulieren en notificaties.

### 1.3. Samenwerkingspartners

Deze handreiking en de bijbehorende schermvoorbeelden zijn een samenwerking van VNGR met het NL Design System kernteam, (UX) designers uit de NL Design System Community en met name de UX designer van Gemeente Den Haag, waar al veel onderzoek gedaan is naar de gebruikersvriendelijkheid van notificaties.

## 2 Achtergrond Wmebv

### 2.1. Wmebv in het kort
In de Handreiking van Het Ministerie van Binnenlandse Zaken in samenwerking met Logius wordt het doel van deze wet helder benoemd:

> De regering wil in het kader van de digitaal werkende overheid komen tot de implementatie van het wetsvoorstel modernisering elektronisch bestuurlijk verkeer. Met name de huidige regel dat een bestuursorgaan verkeer via de elektronische weg moet toestaan en dus ook kan uitsluiten, wordt als verouderd ervaren. Kabinetsbeleid is daarom dat bedrijven en burgers zaken die ze met de overheid doen – zoals het aanvragen van een vergunning – digitaal moeten kunnen afhandelen. Elektronisch bestuurlijk verkeer kan bijdragen aan de vermindering van administratieve lasten van burgers en bestuurlijke lasten van bestuursorganen. De wet neemt belemmeringen weg en stelt enkele randvoorwaarden aan de modernisering en digitalisering van de werkprocessen binnen de publieke sector. Burgers en bedrijven krijgen het recht (niet de plicht) om ieder formeel bericht elektronisch aan de overheid te zenden. Bij gebruik van de elektronische weg gelden er nieuwe waarborgen, waardoor nog meer rechtsbescherming wordt gerealiseerd. Tegelijkertijd houden bestuursorganen ruimte om digitale processen af te stemmen op de eigen organisatie. Om een compacte, efficiënte overheid te realiseren met hoogwaardige dienstverlening, is digitalisering een vereiste en is het digitale kanaal het voorkeurskanaal. Het uitgangspunt is: digitaal waar het kan. Het doel van de Wmebv is om regels over elektronisch bestuurlijk verkeer te moderniseren en burgers en bedrijven het recht te geven om elektronisch zaken te doen met de overheid. Degenen die dat willen moeten voor het digitale kanaal kunnen kiezen in hun contact met de overheid. Om te waarborgen dat iedereen met de overheid kan (blijven) communiceren, is het van belang dat communicatie langs de papieren weg mogelijk blijft. En dat de provincie een inclusief beleid voor ondersteuning van bepaalde doelgroepen gaat uitvoeren.

Bron: [Handreiking implementatie Wet modernisering elektronisch bestuurlijk verkeer (Awb) 2023.](https://www.digitaleoverheid.nl/wp-content/uploads/sites/8/2017/04/Handreiking-implementatie-Wet-modernisering-elektronisch-bestuurlijk-verkeer-2023.pdf)

#### 2.1.2 Bestuurlijk verkeer

Voordat dieper ingegaan wordt over de Wmebv, is het belangrijk om aan te geven om wat voor berichtenverkeer het gaat in de Wmebv. In de diverse documentatie betreft de Wmebv wordt er op verschillende manieren gerefereerd naar het 'Elektronisch Bestuurlijk Verkeer''. Dit verkeer, in de vorm van digitale berichten, wordt in diverse documentatie ook wel 'Officiële berichten', 'Formele berichten' en 'Formeel officiële berichten' genoemd. In alle gevallen wordt hetzelfde bedoeld. In deze handreiking wordt de term 'Formele berichten' aangehouden. Met het Elektronische Bestuurlijk Verkeer worden dus de 'Formele berichten' bedoeld en deze verwijzen doorgaans naar officiële communicatie tussen verschillende bestuurlijke niveaus binnen een overheid. Deze berichten bevatten vaak belangrijke mededelingen, beslissingen, of andere informatie van juridische of bestuurlijke aard. Enkele veelvoorkomende voorbeelden:

* Berichten die deel uit maken van een procedure of besluit
* een klacht
* anders krachtens wettelijk voorschrift voorgeschreven bericht. Bijvoorbeeld een melding.

Niet-officieel bestuurlijke berichten zijn alle andere berichten zoals informele contacten.

Het exacte bereik en de aard van Officiële berichten kunnen sterk variëren, dus het is belangrijk om de specifieke wetgeving en bestuurlijke structuren in overweging te nemen om een vollediger beeld te krijgen van welke producten onder deze term vallen. Voor deze handreiking is het echter van belang het verschil tussen niet officiële berichten en officiële berichten aan te duiden, om zo duidelijk te maken dat de Wmebv niet voor alle processen/producten geldt maar enkel voor de officiële berichten. Voor meer verdieping in de juridische aspecten wordt verwezen naar de video-opname van [Kennissessie 1:  Juridisch Aspecten](https://youtu.be/7Vujk18JA-g) van 9 oktober 2023, die te vinden is op de website: [VNG webinars en kennissessies](https://vng.nl/wmebv-webinars-en-kennissessies) 

En voor meer informatie over een mogelijke aanpak voor de implementatie van de Wmebv wordt verwezen naar dit [Stappenplan](https://vng.nl/artikelen/stappenplan-wet-mebv) ter ondersteuning, waarin de volgende onderwerpen worden behandeld:

**Digitalisering van de dienstverlening**
1. Wat vraagt de Wmebv?
2. Hoe kan ik het aanpakken?
3. Slim digitaliseren met de [omnichannelaanpak](https://vng.nl/omnichannel).
4. Analyse huidige digitale kanalen (met behulp de [Uniforme Productnamen Lijst](https://vng.nl/projecten/uniforme-productnamen-lijst-upl))
5. Besluit en communiceer de gekozen kanalen.
6. Bepaal uw beleid t.a.v. een ([Omnichannel](https://vng.nl/omnichannel)) kanaalstrategie.
7. Aan de gang met implementeren.

**Zorgplicht bij de dienstverlening**
1. Bepaal welke belemmeringen inwoners ervaren
2. Bepaal hoe u belemmeringen kunt wegnemen.
3. Leg uw keuzes voor zorgplicht vast in een beleidsdocument.
4. Communiceer hoe uw gemeente ondersteunt bij de dienstverlening.


> TODO: Geef een overzicht van de Wet en benadruk de relevante secties met betrekking tot e-formulieren en notificaties.
> (Diagram Hendrik) + verwijzingen naar BZK\_Deloitte
> (big picture Wmebv - klantreis) (Figma voorbeeld getoetst met Juliette van der Jagt en op basis van Service Blue print Vincent van Beek)

#### 2.1.3 Belangrijkste aspecten van de Wmebv

![wmebv-schema.png](.media/img_7.png)
De aspecten van de Wmebv zijn op te delen in onder andere een aantal fasen waarin een formeel officieel bericht zich bevindt:

* Fase: Voor ontvangst
    * De Wmebv regelt dat Formele berichten digitaal ontvangen kunnen worden. Dat kan op verschillende manieren voorzien worden:
        * Een generiek contactformulier met upload mogelijkheid (Later in deze handreiking wordt een voorbeeld gedeeld.)
        * E-mail kanaal (maar daar zijn de meningen over verdeeld...)
        * Specifiek webformulier met DigiD / e-Herkenning
        * Via een MijnOmgeving
        * Via een Berichtenbox (Bijvoorbeeld MijnOverheid)
    * De Wmebv regelt dat instanties de wijze van indienen bekend maken door kanalen aan te wijzen en dit bijvoorbeeld vast te leggen in een aanwijzingsbesluit. En de burgers te informeren over het aangewezen digitale kanaal.
    * het is in tevens van belang dat de digitale weg veilig is. Daarbij mogen Belastende of onveilige berichten worden geweigerd.
    * Ook mogen er geen technische eisen gesteld worden die onnodig belemmerend zijn
    * Er mogen geen gegevens afgedwongen worden zonder grondslag. Alleen noodzakelijke gegevens mogen worden uitgevraagd.
    * Tot slot heeft de gemeente de bevoegdheid tot het verlengen van de indieningstermijn bij storing en dient dit bekend te maken op bijvoorbeeld de website.
* Fase: Na ontvangst
    * De Wmebv regelt dat er ontvangstbevestiging verstuurd moet worden. Indien berichten intern doorgeleid zijn of afgewezen zijn, dient dit medegedeeld te worden.
    * Intern doorgeleiden is verplicht als:
        * Het bericht zonder nadere bewerking behandeld kan worden
        * Het bezwaarschrift of beroepsschrift is
        * Voor het type bericht geen wijze van verzending is aangewezen
        * Aanvang wettelijke behandeltermijn opschuift naar tijdstip van het intern doorleiden
        * Mededelingen aan de afzender van het doorgeleiden en tijdstip waarop de termijn aanvangt
    * De Wmebv regelt ook dat indien een bericht verkeerd is ingezonden, en om die reden is afgewezen, dat er een mededeling aan de afzender gezonden moet worden waarin vermeld wordt wat de juiste wijze is.
    * De Wmebv regelt dat ingevulde gegevens van een e-formulier terug-getoond moeten worden. Hetzij via:
        * een download mogelijkheid tijdens het aanvraagproces
        * inzage via een MijnOmgeving
        * het toezenden van het afschrift
* Tot slot dient de gemeente bewijslast te hebben, dat betekent dat een systeem moet zijn waarin gegevens gelogd worden.
* Fase: Uitgaand
    * De Wmebv regelt dat als er genotificeerd wordt, dat er een aantal zaken aangeduid moeten worden:
        * de afzender
        * de aard van het bericht (Bijv. ontvangstbevestiging, beschikking, betalingsverplichting etc.)
        * en een reactietermijn
* Indien een bericht of notificatie niet bezorgd kan worden (een bounce) dan moet het minimaal eenmaal opnieuw verzonden worden.
* De gemeente heeft een inspanningsverplichting om het juiste e-mailadres te achterhalen
* Notificaties moeten op andere wijze verzonden kunnen worden
* De gemeente heeft tevens een bewijslast en moet het volgende kunnen bewijzen:
    * Het tijdstip van verzending of ontvangst
    * De verzending met de samenhangende ontvangstbevestiging of notificatie
    * Tijdstip inlog geadresseerde om kennis te nemen van een aan hem gezonden bericht
    * Ontvangen meldingen van formele berichten die niet konden worden bezorgd
* Zorgplicht
    * De Wmebv regelt tevens een zorgplicht voor passende ondersteuning bij communicatie.
    * Passende ondersteuning:
        * Afgestemd op de doelgroepen en hun vaardigheden (lezen, schrijven, omgaan met digitale apparaten)
        * Ondersteuning is generiek (zoals informatie op een website) en persoonlijk (Zoals hulp aan de telefoon of balie)
        * Maatwerk is niet verplicht
        * Beleid opstellen en publiceren op de website (bijvoorbeeld regels of een handreiking)
    * Hoe inkaderen
        * Wat is de visie op dienstverlening?
        * Data over klantgedrag samenbrengen
        * Begrijpen wat de belemmeringen zijn
        * Beleid maken op passende ondersteuning

<br>
#### 2.1.3 Samengevat in vier punten

De Wmebv is een belangrijk element in de bredere digitale transformatie van overheidsdiensten in Nederland en het is ontworpen om de overgang naar een meer digitaal georiënteerd bestuurlijk verkeer te vergemakkelijken.

* Wmebv is een wijziging van de Algemene Wet Bestuursrecht
* Wmebv geeft het recht op digitaal communiceren met bestuursorganen
* Wmebv stelt het openstellen van digitale kanalen verplicht, voor ieder formeel bestuurlijk bericht gericht aan het bestuursorgaan
* Wmebv resulteert in het aanpassen van digitale kanalen zodat het aan de wettelijk gestelde eisen voldoet.

Zie voor een zeer uitgebreide toelichting op de Wmebv: [Handreiking implementatie Wet modernisering elektronisch bestuurlijk verkeer (Awb) 2023.](https://www.digitaleoverheid.nl/wp-content/uploads/sites/8/2017/04/Handreiking-implementatie-Wet-modernisering-elektronisch-bestuurlijk-verkeer-2023.pdf)

## UX Ontwerpcriteria voor E-formulieren en Notificaties
## Praktische Toepassing: Onze Aanpak in de Praktijk
### A. Project Achtergrond en Doelstelling
### B. Ontwerp in Figma
### C. Development en Code Snippets (Verwijzing)
### D. Usability Tests en Resultaten
# Geleerde Lessen en Aanbevelingen
# Aanvullende Bronnen en Links voor Verdieping