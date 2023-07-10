Van ‘legacy’-metadata naar RDA-entiteiten {#van-legacy}
=====================

De introductie van een nieuwe catalogiseerstandaard stelt bibliotheekinstellingen voor de opgave om hun bestaande bibliografische metadata (‘legacy’-metadata) daarmee in overeenstemming te brengen. 

In de ideale wereld wordt bibliografische metadata gecreëerd en beheerd in een catalogiseersysteem dat RDA-entiteiten volledig ondersteunt. Weinig instellingen zullen nu of in de nabije toekomst van dergelijke catalogiseersystemen gebruikmaken. Ook kennis van RDA en de bijbehorende beschrijvingsregels zijn niet altijd aanwezig binnen bibliotheekorganisaties. 
Toch kunnen RDA-entiteiten ook al afgeleid worden van niet volgens RDA- regels ingevoerde (bestaande of nieuwe) metadata. Deze metadata moet dan wel aan een aantal eisen voldoen. Deze minimale data-eisen worden in het volgende toegelicht. 

## Stappenplan bibliografische metadata 
Als de basiskwaliteit van bibliografische metadata op orde is dan kunnen vervolgstappen voor het herkennen van RDA-entiteiten gezet worden. 

Het stappenplan valt uiteen in twee fasen: 

1. In de eerste fase wordt de eigen bibliografische metadata geanalyseerd en waar nodig verbeterd. Deze fase is nodig om de basiskwaliteit van de bibliografische metadata op orde te brengen en te toetsen aan het toepassingsprofiel. Deze stappen zullen door de instelling zelf uitgevoerd moeten worden. 
 
2. In de tweede fase wordt de bibliografische metadata gekoppeld aan gezaghebbende RDA- entiteiten. De KB zal als nationale bibliotheek in de nabije toekomst waarschijnlijk de entiteiten van de Nederlandse Bibliografie (`Work`, `Expression`, `Manifestation`, `Agent` en ook [Persona](#persona-in-rda)) gezaghebbend publiceren. Als eerste collecties zullen monografische romans en kinderboeken op deze manier gepubliceerd gaan worden. Zo worden de vervolgstappen van fase 2 mogelijk: het koppelen van de eigen bibliografische metadata aan de `Works`, `Expressions`, `Agents` (en eventueel ook de `Manifestations`) van de KB. Hoe beter de kwaliteit van de aangeboden metadata, hoe betrouwbaarder en automatischer deze ‘entiteiten-*matching*’ zal zijn. 

### Fase 1: stappen voor op orde brengen basiskwaliteit metadata 

 
- **Stap 1:** Selecteer de bibliografische metadata van de publicaties die binnen de scope van voorliggend profiel valt vallen,  
- **Stap 2:** Controleer deze dataset aan de hand van de minimale metadata-eisen (*zie tabel 1.*),  
- **Stap 3:** Voer waar nodig opschoonacties en normalisaties op de metadata uit,  
- **Stap 4:** Toets de opgeschoonde metadata aan het RDA Toepassingsprofiel Monografieën 

Controleer per RDA-entiteit of de verplichte gegevens aanwezig zijn in de titelbeschrijvingen. Deze toetsing geeft inzicht in de haalbaarheid van de herkenning van de entiteiten op basis van de metadata. 
 
### Fase 2: (toekomstige) vervolgstappen voor het herkennen en vastleggen van RDA-entiteiten 
 
- **Stap 5:** Toetsing van de eigen opgeschoonde minimale metadata (of de eigen RDA-entiteiten) aan het nog te realiseren KB-register met gezaghebbende RDA-entiteiten. Daarvoor zal de KB de RDA-entiteiten gezaghebbend moeten gaan publiceren en een "RDA Entity Finder"-dienst ontwikkelen.  
- **Stap 6:** Evaluatie en half-automatische/handmatige verwerking van de resultaten.  
- **Stap 7:** Opnemen van de URI’s van de (gezaghebbende KB) RDA-entiteiten op in de eigen metadatabron. 


### Minimale data-eisen 
Voor het herkennen van de RDA-entiteiten Work, Expression, Manifestation en Item, spelen een beperkt aantal gegevens een rol. Het betreft bibliografische informatie-eenheden die van oudsher al vastgelegd worden in bibliografische beschrijvingen, maar die niet altijd afzonderlijk te herkennen zijn, bijvoorbeeld omdat ze als ongestructureerde tekst in een annotatie opgenomen zijn (denk aan de oorspronkelijke titel bij een vertaling), of doordat bij invoer geen gebruik gemaakt is van gecontroleerde lijsten (en tikfouten ontstaan zijn).  

Het is raadzaam of vaak zelfs noodzakelijk de inhoud van onderstaande in de tabel opgenomen informatie-eenheden op te schonen en/of te normaliseren om de RDA-entiteiten herkenning mogelijk te maken. 

Bij de omschrijving van de informatie-eenheden is voor de herkenbaarheid zoveel mogelijk gebruik gemaakt van FOBID/ISBD omschrijvingen. Daarnaast zijn de informatie-eenheden (waar mogelijk) gekoppeld aan de RDA-omschrijving van het overeenkomstige RDA-element. In de kolom VES/SES wordt aangegeven of een controlled vocabulary (*Vocabulary Encoding Scheme* of *VES* in RDA-terminologie) of een gestructureerde tekenreeks (*String Encoding Scheme* of *SES* in RDA-terminologie), gevolgd moet zijn of eventueel afgeleid kan worden. Met andere woorden, bij deze informatie-eenheden is het van belang dat de waardes consistent en/of gestructureerd ingevoerd zijn. Denk bijvoorbeeld aan land- en taalcodes of het gestructureerd opnemen van namen zodat voor- en achternaam onderscheiden kunnen worden. 

In de kolom 'RDA entiteit' wordt aangegeven bij welke WEMI-entiteit de informatie-eenheden horen. In de tabel zijn alleen de minimaal benodigde gegevens voor het herkennen van de WEMI-entiteiten opgenomen (zie voor een volledig overzicht van de informatie-eenheden per WEMI-entiteit [TODO: het Excel-bestand met het Toepassingsprofiel](TODO)). 


<table class='data'>
    <caption>*Tabel 1: Minimale metadata voor de herkenning van de WEMI-entiteiten van RDA*</caption>
    <thead>
        <tr>
            <th>Informatie-eenheid</th>
            <th>Toelichting</th>
            <th>Toelichting RDA</th>
            <th>Verpl.?</th>
            <th>VES/SES</th>
            <th>RDA Entiteit</th>
            <th>Voorbeelden</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>**achternaam en voornaam of voorletters creator(s)**</td>
            <td>primair verantwoordelijke(n)voor de inhoud van de publicatie</td>
            <td>`rdaw:P10065` &quot;*creator agent of work*&quot;</td>
            <td>ja</td>
            <td>ja, om achternaam te kunnen selecteren</td>
            <td>`Work`</td>
            <td>&quot;Couperus, Louis&quot;</td>
        </tr>
        <tr>
            <td>**rol creator(s)**</td>
            <td>rol primair verantwoordelijke(n)</td>
            <td>*subproperties* van `rdaw:P10065` &quot;*creator agent of work*&quot;</td>
            <td>indien bekend</td>
            <td>ja</td>
            <td>`Work`</td>
            <td>aut (author), art (artist)</td>
        </tr>
        <tr>
            <td>**oorspronkelijke titel**</td>
            <td>titel van de eerste editie</td>
            <td>`rdaw:P10088` &quot;*title of work*&quot;</td>
            <td>ja</td>
            <td>nee</td>
            <td>`Work`</td>
            <td>&quot;Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>**alternatieve titel**</td>
            <td></td>
            <td>`rdaw:P10086` &quot;*variant title of work*&quot;</td>
            <td>indien bekend</td>
            <td>nee</td>
            <td>`Work`</td>
            <td>&quot;Max Havelaar&quot;</td>
        </tr>
        <tr>
            <td>**type inhoud**</td>
            <td>communicatievorm (zie ook de [RDA content types](http://www.rdaregistry.info/termList/RDAContentType/))</td>
            <td>`rdae:P20001` &quot;*content type*&quot;</td>
            <td>ja</td>
            <td>ja</td>
            <td>`Expression`</td>
            <td>&quot;text&quot;, &quot;spoken word&quot;</td>
        </tr>
        <tr>
            <td>**taal publicatie**</td>
            <td>gebruik een taalcode met twee tekens volgens ISO 639-1 (2002) of drie tekens volgens ISO 639-2 (1998), ISO 639-3 (2007) of ISO 639-5 (2008)</td>
            <td>`rdae:P20006` &quot;*language of expression*&quot;</td>
            <td>ja</td>
            <td>ja</td>
            <td>`Expression`</td>
            <td>&quot;nl&quot;, &quot;nl-be&quot;</td>
        </tr>
        <tr>
            <td>**titel publicatie**</td>
            <td>kan samenvallen met de oorspronkelijke titel (&quot;*title of work*&quot;), bij een vertaling wijkt deze daar meestal van af (&quot;*title of expression*&quot;)</td>
            <td>`rdaw:P10088` &quot;title of work&quot; ,  `rdae:P20312` &quot;*title of expression*&quot;</td>
            <td>indien aanwezig</td>
            <td>nee</td>
            <td>`Work`, `Expression`</td>
            <td>&quot;The black lake&quot; (een vertaling van &quot;Oeroeg&quot;)</td>
        </tr>
        <tr>
            <td>**achternaam inhoudelijke bijdrager aan publicatie**</td>
            <td>betreft bijdragers die een inhoudelijke bijdrage aan de creatieve of intellectuele inhoud van de publicatie geleverd hebben</td>
            <td>`rdae:P2005` &quot;*creator agent of expression*&quot;</td>
            <td>indien aanwezig</td>
            <td>ja, om achternaam auteur te kunnen selecteren</td>
            <td>`Expression`</td>
            <td>&quot;Noble, Philippe&quot;</td>
        </tr>
        <tr>
            <td>**rol bijdrager**</td>
            <td></td>
            <td>`rdae:P20053`, zie de subproperties</td>
            <td>indien bekend</td>
            <td>ja</td>
            <td>`Expression`</td>
            <td>&quot;trl&quot; (translator)</td>
        </tr>
        <tr>
            <td>**drager / carrier**</td>
            <td>aanduiding drager van de publicatie (zie ook de [RDA carrier types](http://www.rdaregistry.info/termList/RDACarrierType/))</td>
            <td>`rdam:P30001` &quot;*carrier type*&quot;</td>
            <td>ja</td>
            <td>ja</td>
            <td>`Manifestation`</td>
            <td>&quot;band&quot;, &quot;microfiche&quot;</td>
        </tr>
        <tr>
            <td>**jaar van publicatie**</td>
            <td></td>
            <td>`rdam:P30011` &quot;*date of publication*&quot;</td>
            <td>ja</td>
            <td>ja</td>
            <td>`Manifestation`</td>
            <td>&quot;1969&quot;</td>
        </tr>
        <tr>
            <td>**uitgever**</td>
            <td>(eerste) uitgever of host</td>
            <td>`rdam:P30176` &quot;name of publisher&quot;</td>
            <td>ja</td>
            <td>nee</td>
            <td>`Manifestation`</td>
            <td>&quot;Pandora&quot;</td>
        </tr>
        <tr>
            <td>**medium type**</td>
            <td>drukt uit welk type apparaat vereist is om de inhoud van een bron te bekijken, af te spelen etc. (zie ook de [RDA media types](http://www.rdaregistry.info/termList/RDAMediaType/))</td>
            <td>`rdam:P30002` &quot;*has media type*&quot;</td>
            <td>indien bekend</td>
            <td>ja</td>
            <td>`Manifestation`</td>
            <td>&quot;computer&quot;, &quot;zonder medium&quot; (bij een gedrukte publicatie)</td>
        </tr>
        <tr>
            <td>**wijze van uitgave / mode of issuance**</td>
            <td>geeft aan of de publicatie als eendelig document (al dan niet in reeks) of als onderdeel van een meerdelige publicatie verschenen is (zinvol is de context of bron van de identifier aan te duiden met een prefix, zoals "ISBN: ")</td>
            <td>`rdam:P30003` &quot;*has mode of issuance*&quot;</td>
            <td>indien bekend</td>
            <td>ja</td>
            <td>`Manifestation`</td>
            <td>&quot;eendelig document&quot; , &quot;zelfstandige deeltitel MP&quot;</td>
        </tr>
        <tr>
            <td>**identifier**</td>
            <td>identifier voor de publicatie</td>
            <td>`rdam:P30004` &quot;*identifier for manifestation*&quot;</td>
            <td>indien bekend</td>
            <td>nee</td>
            <td>`Manifestation`</td>
            <td>&quot;ISBN:  9789023408017&quot; [^5]</td>
        </tr>
        <tr>
            <td>**paginering**</td>
            <td>paginering, omvang van de publicatie</td>
            <td>`rdam:P30182` &quot;*extent of manifestation*&quot;</td>
            <td>indien bekend</td>
            <td>ja</td>
            <td>`Manifestation`</td>
            <td>&quot;80 p.&quot;</td>
        </tr>
        <tr>
            <td>**plaats van uitgave**</td>
            <td></td>
            <td>`rdam:P30182` &quot;*place of publication*&quot;</td>
            <td>indien bekend</td>
            <td>nee</td>
            <td>`Manifestation`</td>
            <td>&quot;Amsterdam&quot;</td>
        </tr>
        <tr>
            <td>**persistente identifier exemplaar**</td>
            <td>moet uniek zijn in combinatie met de instellingsnaam en het land waar de instelling gevestigd is (meer informatie over persistente identifiers, zie [Netwerk digitaal Erfgoed](https://netwerkdigitaalerfgoed.nl/activiteiten/persistent-identifiers/))</td>
            <td>`rdai:P40001` &quot;*has identifier for item*&quot;</td>
            <td>ja</td>
            <td>nee</td>
            <td>`Item`</td>
            <td>&quot;2365290&quot; (als signatuur), &quot;urn:nbn:nl:kb-1684989030400&quot; (NBN (National Bibliographic Number), &quot;MMKB18B:060765000&quot; (URN - Uniform Resource Name)</td>
        </tr>
    </tbody>
</table>

Zie ook voorbeelden:

* [een traditionele titelbeschrijving, met minimale metadata voor RDA-entiteiten](#traditioneel_minimaal1)
* [een traditionele titelbeschrijving van een vertaling, met minimale metadata voor RDA-entiteiten](#traditioneel_minimaal2)
