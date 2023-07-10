Van 'legacy'-metadata naar RDA-entiteiten {#van-legacy}
=====================

De introductie van een nieuwe catalogiseerstandaard stelt bibliotheekinstellingen voor de opgave om hun bestaande bibliografische metadata ('legacy'-metadata) daarmee in overeenstemming te brengen. 

In de ideale wereld wordt bibliografische metadata gecreëerd en beheerd in een catalogiseersysteem dat RDA-entiteiten volledig ondersteunt. Weinig instellingen zullen nu of in de nabije toekomst van dergelijke catalogiseersystemen gebruikmaken. Ook kennis van RDA en de bijbehorende beschrijvingsregels zijn niet altijd aanwezig binnen bibliotheekorganisaties. 
Toch kunnen RDA-entiteiten ook al afgeleid worden van niet volgens RDA- regels ingevoerde (bestaande of nieuwe) metadata. Deze metadata moet dan wel aan een aantal eisen voldoen. Deze minimale data-eisen worden in het volgende toegelicht. 

## Stappenplan bibliografische metadata 
Als de basiskwaliteit van bibliografische metadata op orde is dan kunnen vervolgstappen voor het herkennen van RDA-entiteiten gezet worden. 

Het stappenplan valt uiteen in twee fasen: 

1. In de eerste fase wordt de eigen bibliografische metadata geanalyseerd en waar nodig verbeterd. Deze fase is nodig om de basiskwaliteit van de bibliografische metadata op orde te brengen en te toetsen aan het toepassingsprofiel. Deze stappen zullen door de instelling zelf uitgevoerd moeten worden. 
 
2. In de tweede fase wordt de bibliografische metadata gekoppeld aan gezaghebbende RDA- entiteiten. De KB zal als nationale bibliotheek in de nabije toekomst waarschijnlijk de entiteiten van de Nederlandse Bibliografie (`Work`, `Expression`, `Manifestation`, `Agent` en ook [*Persona*](Persona_in_RDA.md)) gezaghebbend publiceren. Als eerste collecties zullen monografische romans en kinderboeken op deze manier gepubliceerd gaan worden. Zo worden de vervolgstappen van fase 2 mogelijk: het koppelen van de eigen bibliografische metadata aan de `Works`, `Expressions`, `Agents` (en eventueel ook de `Manifestations`) van de KB. Hoe beter de kwaliteit van de aangeboden metadata, hoe betrouwbaarder en automatischer deze ‘entiteiten-*matching*’ zal zijn. 

### Fase 1: stappen voor op orde brengen basiskwaliteit metadata 

 
**Stap 1:** Selecteer de bibliografische metadata van de publicaties die binnen de scope van voorliggend profiel valt vallen,  
**Stap 2:** Controleer deze dataset aan de hand van de minimale metadata-eisen (*zie tabel 1.*),  
**Stap 3:** Voer waar nodig opschoonacties en normalisaties op de metadata uit,  
**Stap 4:** Toets de opgeschoonde metadata aan het RDA Toepassingsprofiel Monografieën 
Controleer per RDA-entiteit of de verplichte gegevens aanwezig zijn in de titelbeschrijvingen. Deze toetsing geeft inzicht in de haalbaarheid van de herkenning van de entiteiten op basis van de metadata. 

 
### Fase 2: (toekomstige) vervolgstappen voor het herkennen en vastleggen van RDA-entiteiten 
 
**Stap 5:** Toetsing van de eigen opgeschoonde minimale metadata (of de eigen RDA-entiteiten) aan het nog te realiseren KB-register met gezaghebbende RDA-entiteiten. Daarvoor zal de KB de RDA-entiteiten gezaghebbend moeten gaan publiceren en een "RDA Entity Finder"-dienst ontwikkelen.  
**Stap 6:** Evaluatie en half-automatische/handmatige verwerking van de resultaten.  
**Stap 7:** Opnemen van de URI’s van de (gezaghebbende KB) RDA-entiteiten op in de eigen metadatabron. 


#### Minimale data-eisen 
Voor het herkennen van de RDA-entiteiten Work, Expression, Manifestation en Item, spelen een beperkt aantal gegevens een rol. Het betreft bibliografische informatie-eenheden die van oudsher al vastgelegd worden in bibliografische beschrijvingen, maar die niet altijd afzonderlijk te herkennen zijn, bijvoorbeeld omdat ze als ongestructureerde tekst in een annotatie opgenomen zijn (denk aan de oorspronkelijke titel bij een vertaling), of doordat bij invoer geen gebruik gemaakt is van gecontroleerde lijsten (en tikfouten ontstaan zijn).  

Het is raadzaam of vaak zelfs noodzakelijk de inhoud van onderstaande in de tabel opgenomen informatie-eenheden op te schonen en/of te normaliseren om de RDA-entiteiten herkenning mogelijk te maken. 

Bij de omschrijving van de informatie-eenheden is voor de herkenbaarheid zoveel mogelijk gebruik gemaakt van FOBID/ISBD omschrijvingen. Daarnaast zijn de informatie-eenheden (waar mogelijk) gekoppeld aan de RDA-omschrijving van het overeenkomstige RDA-element. In de kolom VES/SES wordt aangegeven of een controlled vocabulary (*Vocabulary Encoding Scheme* of *VES* in RDA-terminologie) of een gestructureerde tekenreeks (*String Encoding Scheme* of *SES* in RDA-terminologie), gevolgd moet zijn of eventueel afgeleid kan worden. Met andere woorden, bij deze informatie-eenheden is het van belang dat de waardes consistent en/of gestructureerd ingevoerd zijn. Denk bijvoorbeeld aan land- en taalcodes of het gestructureerd opnemen van namen zodat voor- en achternaam onderscheiden kunnen worden. 

In de kolom 'RDA entiteit' wordt aangegeven bij welke WEMI-entiteit de informatie-eenheden horen. In de tabel zijn alleen de minimaal benodigde gegevens voor het herkennen van de WEMI-entiteiten opgenomen (zie voor een volledig overzicht van de informatie-eenheden per WEMI-entiteit [TODO: het Excel-bestand met het Toepassingsprofiel](TOD)). 

*Tabel 1: Minimale metadata voor de herkenning van de WEMI-entiteiten van RDA*

| Informatie-eenheid | Toelichting | Toelichting RDA | Verpl.? | VES/SES | RDA Entiteit | Voorbeelden |
| ------------------ | ----------- | --------------- | --------- | ------- | ------------ | ----------- |
| **achternaam en voornaam of voorletters creator(s)** | primair verantwoordelijke(n)voor de inhoud van de publicatie | `rdaw:P10065` "*creator agent of work*" | ja | ja, om achternaam te kunnen selecteren | `Work` | "Couperus, Louis" |
| **rol creator(s)** | rol primair verantwoordelijke(n) | *subproperties* van `rdaw:P10065` "*creator agent of work*" | indien bekend  | ja | `Work` | aut (author), art (artist) |
| **oorspronkelijke titel** | titel van de eerste editie | `rdaw:P10088` "*title of work*" | ja | nee | `Work`  | "Aan den weg der vreugde" | 
| **alternatieve titel** | | `rdaw:P10086` "*variant title of work*" | indien bekend | nee | `Work` | "Max Havelaar" | 
| **type inhoud** | communicatievorm  | `rdae:P20001` "*content type*" | ja | ja | `Expression` |  "text", "spoken word" [^1] | 
| **taal publicatie** | | `rdae:P20006` "*language of expression*" | ja | ja | `Expression` |  "nl", "nl-be" [^2] |
| **titel publicatie** | kan samenvallen met de oorspronkelijke titel ("*title of work*"), bij een vertaling wijkt deze daar meestal van af ("*title of expression*") | `rdaw:P10088` "title of work" ,  `rdae:P20312` "*title of expression*" | indien aanwezig | nee | `Work`, `Expression` |  "The black lake" (een vertaling van "Oeroeg") |
| **achternaam inhoudelijke bijdrager aan publicatie** | betreft bijdragers die een inhoudelijke bijdrage aan de creatieve of intellectuele inhoud van de publicatie geleverd hebben | `rdae:P2005` "*creator agent of expression*" |indien aanwezig | ja, om achternaam auteur te kunnen selecteren | `Expression` | "Noble, Philippe" |
| **rol bijdrager** | | `rdae:P20053`, zie de subproperties | indien bekend  | ja | `Expression` |  "trl" (translator) | 
| **drager / carrier** | aanduiding drager van de publicatie |`rdam:P30001` "*carrier type*" | ja | ja | `Manifestation` | "band", "microfiche" [^3] |
| **jaar van publicatie** | | `rdam:P30011` "*date of publication*" | ja | ja | `Manifestation` | "1969" |
| **uitgever** | (eerste) uitgever of host | `rdam:P30176` "name of publisher" | ja | nee | `Manifestation` | "Pandora" | 
| **medium type** | drukt uit welk type apparaat vereist is om de inhoud van een bron te bekijken, af te spelen etc. | `rdam:P30002` "*has media type*" |indien bekend | ja | `Manifestation` | "computer", "zonder medium" (bij een gedrukte publicatie) [^4] |
| **wijze van uitgave / mode of issuance** | geeft aan of de publicatie als eendelig document (al dan niet in reeks) of als onderdeel van een meerdelige publicatie verschenen is | `rdam:P30003` "*has mode of issuance*" | indien bekend | ja | `Manifestation` | "eendelig document" , "zelfstandige deeltitel MP" [^5] | 
| **identifier** | identifier voor de publicatie | `rdam:P30004` "*identifier for manifestation*" | indien bekend | nee | `Manifestation` | "ISBN:  9789023408017" [^5] |
| **paginering** | paginering, omvang van de publicatie | `rdam:P30182` "*extent of manifestation*" | indien bekend | ja | `Manifestation` | "80 p." |
| **plaats van uitgave** | | `rdam:P30182` "*place of publication*" | indien bekend | nee | `Manifestation` | "Amsterdam" | 
| **persistente identifier exemplaar** | moet uniek zijn in combinatie met de instellingsnaam en het land waar de instelling gevestigd is [^6] | `rdai:P40001` "*has identifier for item*"  | ja | nee | `Item` | "2365290" (als signatuur), "urn:nbn:nl:kb-1684989030400" (NBN (National Bibliographic Number), "MMKB18B:060765000" (URN - Uniform Resource Name) |

Zie ook voorbeelden:

* [`Traditioneel_minimaal1.md`](examples/Traditioneel_minimaal1.md) : een traditionele titelbeschrijving, met minimale metadata voor RDA-entiteiten.
* [`Traditioneel_minimaal2.md`](examples/Traditioneel_minimaal1.md`) : een traditionele titelbeschrijving van een vertaling, met minimale metadata voor RDA-entiteiten. 


[^1]: zie ook de [RDA content types](http://www.rdaregistry.info/termList/RDAContentType/) 
[^2]: gebruik een taalcode met twee tekens volgens ISO 639-1 (2002) of drie tekens volgens ISO 639-2 (1998), ISO 639-3 (2007) of ISO 639-5 (2008)
[^3]: zie ook de [RDA carrier types](http://www.rdaregistry.info/termList/RDACarrierType/)
[^4]: zie ook de [RDA media types](http://www.rdaregistry.info/termList/RDAMediaType/)
[^5]: zinvol is de context of bron van de identifier aan te duiden met een prefix, zoals "ISBN: "
[^6]: meer informatie over persistente identifiers, zie [Netwerk digitaal Erfgoed](https://netwerkdigitaalerfgoed.nl/activiteiten/persistent-identifiers/) 

 