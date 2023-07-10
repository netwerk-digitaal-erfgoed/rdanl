Toe te passen RDA-kenmerken voor Manifestation-entiteiten {#manifestation-kenmerken}
--------------------

<table class='complex data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>opm.</th>
            <th>range</th>
            <th>vastlegging</th>
            <th>verpl.?</th>
            <th>max.</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td colspan=2>*Appellation:*</td>
            <td>*elementen om de entiteit te benoemen:*</td>
            <td></td>
            <td></td>
            <td>M</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30156](http://rdaregistry.info/Elements/m/P30156)</td>
            <td>**titleProper**</td>
            <td>letterijk overnemen uit de bron zoals het er staat, ook eventuele tikfouten<br>vastleggen als een zin<br>hoofdlettergebruik zoals in de taal van de titel gebruikelijk is<br>bij fouten de gecorrigeerde titel opnemen als **variantTitleOfManifestation**</td>
            <td>`Nomen`</td>
            <td>U</td>
            <td>M</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30128](http://rdaregistry.info/Elements/m/P30128)</td>
            <td>**variantTitleOfManifestation**</td>
            <td>zie bij **titleProper**</td>
            <td>`Nomen`</td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30004](http://rdaregistry.info/Elements/m/P30004)</td>
            <td>**identifierForManifestation**</td>
            <td>systeemonafhankelijke identifier, indien mogelijk persistent, dit is niet de identifier van het metadata record</td>
            <td>`Nomen`</td>
            <td>Id</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td>&quot;urn:isbn:9025499678&quot;</td>
        </tr>
        <tr>
            <td colspan=2>*Coherence:*</td>
            <td>*primaire relaties tussen entiteiten:*</td>
            <td></td>
            <td></td>
            <td>M</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30139](http://rdaregistry.info/Elements/m/P30139)</td>
            <td>**expressionManifested**</td>
            <td></td>
            <td>`Expression`</td>
            <td>S / Id / IRI</td>
            <td>M</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30135](http://rdaregistry.info/Elements/m/P30135)</td>
            <td>**workManifested**</td>
            <td></td>
            <td>`Work`</td>
            <td>S / Id / IRI</td>
            <td>O</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30103](http://rdaregistry.info/Elements/m/P30103)</td>
            <td>**exemplarOfManifestation**</td>
            <td></td>
            <td>`Item`</td>
            <td>S / Id / IRI</td>
            <td>M</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td colspan=2>*General description:*</td>
            <td>*algemene beschrijving (basistoepassingsprofiel):*</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30002](http://rdaregistry.info/Elements/m/P30002)</td>
            <td>**mediaType**</td>
            <td></td>
            <td></td>
            <td>S / IRI</td>
            <td>M</td>
            <td>1</td>
            <td>[RDA Media Type](http://www.rdaregistry.info/termList/RDAMediaType/)</td>
        </tr>
        <tr>
            <td>[rdam:P30003](http://rdaregistry.info/Elements/m/P30003)</td>
            <td>**modeOfIssuance**</td>
            <td></td>
            <td></td>
            <td>S / IRI</td>
            <td>M</td>
            <td>1</td>
            <td>[RDA Mode of Issuance](http://www.rdaregistry.info/termList/ModeIssue/)</td>
        </tr>
        <tr>
            <td>[rdam:P30335](http://rdaregistry.info/Elements/m/P30335)</td>
            <td>**categoryOfManifestation**</td>
            <td>TODO: zijn dit de vormtrefwoorden?</td>
            <td></td>
            <td>U / S / Id / IRI</td>
            <td>O</td>
            <td>1</td>
            <td>[Brinkman Trefwoordenthesaurus](http://data.bibliotheken.nl/id/dataset/brinkman) , [Thema](https://ns.editeur.org/thema/nl)</td>
        </tr>
        <tr>
            <td>[rdam:P30142](http://rdaregistry.info/Elements/m/P30142)</td>
            <td>**otherTitleInformation**</td>
            <td>gebruik voor ondertitel</td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30105](http://rdaregistry.info/Elements/m/P30105)</td>
            <td>**statementOfResponsibilityRelatingToTitleProper**</td>
            <td>TODO waarvoor? / overnemen uit de resource</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30280](http://rdaregistry.info/Elements/m/P30280)</td>
            <td>**manifestationCopyrightStatement**</td>
            <td>datum en bij wie de copyright berust, overnemen uit de bron<br>als alleen een datum bekend is, gebruik dan **copyrightDate**</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30007](http://rdaregistry.info/Elements/m/P30007)</td>
            <td>**copyrightDate**</td>
            <td>datum copyright zoals vermeld in de bron</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td>ISO 8601-1:2019</td>
        </tr>
        <tr>
            <td>[rdam:P30107](http://rdaregistry.info/Elements/m/P30107)</td>
            <td>**editionStatement**</td>
            <td>een vermelding die een editie identificeert waartoe een manifestatie behoort<br>wordt samengesteld uit de volgende elementen: **designationOfEdition**, **designationOfNamedRevisionOfEdition**, **statementOfResponsibilityRelatingToEdition**, **statementOfResponsibilityRelatingToNamedRevisionOfEdition**, als deze elementen apart genoteerd kunnen worden en van toepassing zijn, gebruik deze elementen, indien de informatie als geheel wordt opgenomen, gebruik dan dit element</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30133](http://rdaregistry.info/Elements/m/P30133)</td>
            <td>**designationOfEdition**</td>
            <td>overnemen uit de bron</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30132](http://rdaregistry.info/Elements/m/P30132)</td>
            <td>**designationOfNamedRevisionOfEdition**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30121](http://rdaregistry.info/Elements/m/P30121)</td>
            <td>**statementOfResponsibilityRelatingToEdition**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30118](http://rdaregistry.info/Elements/m/P30118)</td>
            <td>**statementOfResponsibilityRelatingToNamedRevisionOfEdition**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30001](http://rdaregistry.info/Elements/m/P30001)</td>
            <td>**carrierType**</td>
            <td></td>
            <td></td>
            <td>S / Id / IRI</td>
            <td>M</td>
            <td>1</td>
            <td>[RDA Carrier Type](http://www.rdaregistry.info/termList/RDACarrierType/)</td>
        </tr>
        <tr>
            <td>[rdam:P30182](http://rdaregistry.info/Elements/m/P30182)</td>
            <td>**extentOfManifestation**</td>
            <td>o.a. aantal pagina&#39;s</td>
            <td></td>
            <td>S</td>
            <td>M</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30169](http://rdaregistry.info/Elements/m/P30169)</td>
            <td>**dimensions**</td>
            <td>neem op wat nodig is voor het magazijn van fysieke bronnen,  maten in cm., tenzij hoogte &lt; 10 cm, dan in mm.</td>
            <td></td>
            <td>U / S (?)</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30137](http://rdaregistry.info/Elements/m/P30137)</td>
            <td>**noteOnManifestation**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30453](http://rdaregistry.info/Elements/m/P30453)</td>
            <td>**illustrativeContent**</td>
            <td>een indicatie van de soorten expressies van beeldcontent die de hoofd-expressies aanvullen</td>
            <td></td>
            <td>S / IRI</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td>[RDA Illustrative Content](http://www.rdaregistry.info/termList/IllusContent/)</td>
        </tr>
        <tr>
            <td>[rdam:P30309](http://rdaregistry.info/Elements/m/P30309)</td>
            <td>**typeOfBinding**</td>
            <td></td>
            <td></td>
            <td>S / IRI</td>
            <td>O</td>
            <td>&gt;1</td>
            <td>[RDA Type of Binding](http://www.rdaregistry.info/termList/RDATypeOfBinding/)</td>
        </tr>
        <tr>
            <td>[rdam:P30160](http://rdaregistry.info/Elements/m/P30160)</td>
            <td>**termOfAvailability**</td>
            <td>o.a. prijs</td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30111](http://rdaregistry.info/Elements/m/P30111)</td>
            <td>**publicationStatement**</td>
            <td>wordt samengesteld uit de elementen: **placeOfPublication**, name of publisher, **dateOfPublication**. Als deze apart genoteerd kunnen worden en van toepassing zijn, gebruik deze elementen. Indien de informatie als geheel wordt opgenomen, gebruik dan dit aggregerende relement</td>
            <td></td>
            <td>S</td>
            <td>O</td>
            <td>1</td>
            <td>&quot;Spijkenisse : Hageboek, 1998&quot;</td>
        </tr>
        <tr>
            <td colspan=2>*General relationships:*</td>
            <td>*algemene elementen om relaties van de entiteit te beschrijven (basistoepassingsprofiel):*</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30088](http://rdaregistry.info/Elements/m/P30088)</td>
            <td>**placeOfPublication**</td>
            <td>zoals vermeld in de bron. Indien niet bekend, geef aan: &quot;Plaats van uitgave niet vastgesteld&quot; in element **noteOnManifestation**.<br>Zet een plaats tussen vierkante haken als de bron van de informatie niet de `Manifestation` zelf is. [ TODO: willen we dit wel? -&gt; Indien mogelijk herhaal dit element om een identifier of iri van een plaats te geven. Herhaal dit element om een land van uitgave te vermelden, het liefst gestructureerd, met identifier of iri. Indien de identifier van een plaats het land duidelijk aangeeft, dan is een land van uitgave niet nodig]</td>
            <td>`Place`</td>
            <td>U / Id / IRI</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30083](http://rdaregistry.info/Elements/m/P30083)</td>
            <td>**publisherAgent**</td>
            <td>overnemen uit de bron</td>
            <td>`Agent`</td>
            <td>U / Id / IRI</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30011](http://rdaregistry.info/Elements/m/P30011)</td>
            <td>**dateOfPublication**</td>
            <td>indien onbekend, geen datum, jaar of periode wanneer publicatie kan hebben plaatsgevonden</td>
            <td>`Timespan`</td>
            <td>U / S / Id / IRI</td>
            <td>M</td>
            <td>1</td>
            <td>ISO 8601-1:2019</td>
        </tr>
        <tr>
            <td>[rdam:P30321](http://rdaregistry.info/Elements/m/P30321)</td>
            <td>**contributorAgentOfStillImage**</td>
            <td></td>
            <td>`Agent`</td>
            <td>U / S / Id / IRI</td>
            <td>O</td>
            <td>&gt;1</td>
            <td>[Nederlandse Thesaurus van Auteursnamen (NTA)](http://data.bibliotheken.nl/id/dataset/persons) , [NACO - Name Authority Cooperative Program](https://www.loc.gov/aba/pcc/naco/) , [Corporatiethesaurus](http://data.bibliotheken.nl/id/dataset/corps)</td>
        </tr>
        <tr>
            <td>[rdam:P30328](http://rdaregistry.info/Elements/m/P30328)</td>
            <td>**contributorAgentOfText**</td>
            <td></td>
            <td>`Agent`</td>
            <td>U / S / Id / IRI</td>
            <td>O</td>
            <td>&gt;1</td>
            <td>[Nederlandse Thesaurus van Auteursnamen (NTA)](http://data.bibliotheken.nl/id/dataset/persons) , [NACO - Name Authority Cooperative Program](https://www.loc.gov/aba/pcc/naco/) , [Corporatiethesaurus](http://data.bibliotheken.nl/id/dataset/corps)</td>
        </tr>
        <tr>
            <td>[rdam:P30157](http://rdaregistry.info/Elements/m/P30157)</td>
            <td>**titleOfSeries**</td>
            <td>letterlijk overnemen uit de bron, vastleggen als een zin<br> Hoofdlettergebruik zoals in de taal van de titel gebruikelijk is.</td>
            <td>`Nomen`</td>
            <td>U</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30048](http://rdaregistry.info/Elements/m/P30048)</td>
            <td>**relatedManifestationOfManifestation**</td>
            <td></td>
            <td>`Manifestation`</td>
            <td>U / S / Id / IRI</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
           <td colspan=2>*Special description:*</td>
            <td>*Gespecialiseerde elementen om de entiteit te beschrijven:*</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30096](http://rdaregistry.info/Elements/m/P30096)</td>
            <td>**encodingFormat**</td>
            <td>wijze waarop digitale inhoud gecodeerd is</td>
            <td></td>
            <td>U / S / IRI</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td>&quot;html&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30018](http://rdaregistry.info/Elements/m/P30018)</td>
            <td>**fileType**</td>
            <td></td>
            <td></td>
            <td>U / S / IRI</td>
            <td>O</td>
            <td>1</td>
            <td>[RDA File Type](http://rdaregistry.info/termList/fileType)</td>
        </tr>
        <tr>
            <td>[rdam:P30183](http://rdaregistry.info/Elements/m/P30183)</td>
            <td>**fileSize**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30165](http://rdaregistry.info/Elements/m/P30165)</td>
            <td>**numberingOfSequence**</td>
            <td>overnemen uit de bron</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30454](http://rdaregistry.info/Elements/m/P30454)</td>
            <td>**soundContent**</td>
            <td>indicatie van de aanwezigheid of afwezigheid van geluid (NB: In 2025 wordt de wet m.b.t. digitale toegankelijkheid van kracht. Uitgevers worden geacht gegevens daarover aan te leveren. Het is van belang deze op te nemen in de metadata.)</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30456](http://rdaregistry.info/Elements/m/P30456)</td>
            <td>**colourContent**</td>
            <td>indicatie van de aanwezigheid van kleur of grijsschakeringen (NB: In 2025 wordt de wet m.b.t. digitale toegankelijkheid van kracht. Uitgevers worden geacht gegevens daarover aan te leveren. Het is van belang deze op te nemen in de metadata.)</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30452](http://rdaregistry.info/Elements/m/P30452)</td>
            <td>**accessibilityContent**</td>
            <td>indicatie van de soorten expressies die alternatieve zintuiglijke modi bieden om de hoofd-expressie waar te nemen [^14 ]</td>
            <td></td>
            <td>U</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
    </tbody>
</table>
