Uitwerking met RIMMF {#uitwerking-rimmf}
-------------

*Ter illustratie* de volgende beschrijving van een `Work` met bijbehorende `Expressions` en `Manifestations` zoals gegeneerd door \[RIMMF](https://www.rimmf.com/)) (RDA in Many Metadata Formats" - is een hulpmiddel voor MS Windows voor het (leren) werken met RDA.). Hierbij wordt een traditioneel implementatiescenario gevolgd, gebaseerd op (geautoriseerde) ingangen. De identifiers zijn door RIMMF gegeneerd. 

In dit voorbeeld van RIMMF wordt niet de voorgestelde [Persona-aanpak](#persona-in-rda) gevolgd, of de voorgestelde gestructureerde tekenreeksen (SES). Zie de [uitwerking in RDF](../rdf/examples) voor een beschrijving in lijn met de voorgestelde aanpak.

### Work

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdac:Work</td>
        </tr>
        <tr>
            <td>[rdaw:P10002](http://rdaregistry.info/Elements/w/P10002)</td>
            <td>**identifierForWork**</td>
            <td>&quot;kob105&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10223](http://rdaregistry.info/Elements/w/P10223)</td>
            <td>**preferredTitleOfWork**</td>
            <td>&quot;Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10086](http://rdaregistry.info/Elements/w/P10086)</td>
            <td>**variantTitleOfWork**</td>
            <td>&quot;Een vrouw van het noorden&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10331](http://rdaregistry.info/Elements/w/P10331)</td>
            <td>**authorizedAccessPointForWork**</td>
            <td>&quot;Couperus, Louis (1863-1923 | Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10332](http://rdaregistry.info/Elements/w/P10332)</td>
            <td>**variantAccessPointForWork**</td>
            <td>&quot;Couperus, Louis (1863-1923 | Een vrouw van het noorden&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10004](http://rdaregistry.info/Elements/w/P10004)</td>
            <td>**categoryOfWork**</td>
            <td>&quot;romans en novellen&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10365](http://rdaregistry.info/Elements/w/P10365)</td>
            <td>**extensionPlan**</td>
            <td>&quot;static plan&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10078](http://rdaregistry.info/Elements/w/P10078)</td>
            <td>**expressionOfWork**</td>
            <td>&quot;Couperus, Louis (1863-1923) | Aan den weg der vreugde | text | Dutch&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10436](http://rdaregistry.info/Elements/w/P10436)</td>
            <td>**authorPerson**</td>
            <td>&quot;Couperus, Louis (1863-1923)&quot;</td>
        </tr>
        <tr>
            <td>[rdaw:P10219](http://rdaregistry.info/Elements/w/P10219)</td>
            <td>**dateOfWork**</td>
            <td>&quot;1908&quot;</td>
        </tr>
    </tbody>
</table>
</div>

### Expression

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdanl:Expression</td>
        </tr>
        <tr>
            <td>[rdae:P20002](http://rdaregistry.info/Elements/e/P20002)</td>
            <td>**identifierForExpression**</td>
            <td>&quot;kob103&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20313](http://rdaregistry.info/Elements/e/P20313)</td>
            <td>**authorizedAccessPointForExpression**</td>
            <td>&quot;Couperus, Louis (1863-1923) | Aan den weg der vreugde | text | Dutch&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20231](http://rdaregistry.info/Elements/e/P20231)</td>
            <td>**workExpressed**</td>
            <td>&quot;Couperus, Louis (1863-1923 | Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20059](http://rdaregistry.info/Elements/e/P20059)</td>
            <td>**manifestationOfExpression**</td>
            <td>&quot;Aan den weg der vreugde | L.J. Veen | [1908] | volume &quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20006](http://rdaregistry.info/Elements/e/P20006)</td>
            <td>**languageOfExpression**</td>
            <td>&quot;Dutch&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20001](http://rdaregistry.info/Elements/e/P20001)</td>
            <td>**contentType**</td>
            <td>&quot;text&quot;</td>
        </tr>
    </tbody>
</table>
</div>

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdanl:Expression</td>
        </tr>
        <tr>
            <td>[rdae:P20002](http://rdaregistry.info/Elements/e/P20002)</td>
            <td>**identifierForExpression**</td>
            <td>&quot;kob109&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20313](http://rdaregistry.info/Elements/e/P20313)</td>
            <td>**authorizedAccessPointForExpression**</td>
            <td>&quot;Couperus, Louis (1863-1923) | Een vrouw van het noorden | text | Dutch&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20231](http://rdaregistry.info/Elements/e/P20231)</td>
            <td>**workExpressed**</td>
            <td>&quot;Couperus, Louis (1863-1923 | Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20315](http://rdaregistry.info/Elements/e/P20315)</td>
            <td>**preferredTitleOfExpression**</td>
            <td>&quot;Een vrouw van het noorden&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20059](http://rdaregistry.info/Elements/e/P20059)</td>
            <td>**manifestationOfExpression**</td>
            <td>&quot;Een vrouw van het noorden | Pandorra | [1999] | volume | 2e dr&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20006](http://rdaregistry.info/Elements/e/P20006)</td>
            <td>**languageOfExpression**</td>
            <td>&quot;Dutch&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20001](http://rdaregistry.info/Elements/e/P20001)</td>
            <td>**contentType**</td>
            <td>&quot;text&quot;</td>
        </tr>
    </tbody>
</table>
</div>

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdanl:Expression</td>
        </tr>
        <tr>
            <td>[rdae:P20002](http://rdaregistry.info/Elements/e/P20002)</td>
            <td>**identifierForExpression**</td>
            <td>&quot;kob111&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20313](http://rdaregistry.info/Elements/e/P20313)</td>
            <td>**authorizedAccessPointForExpression**</td>
            <td>&quot;Am Wege der Freude | text | German | Otten, Else (1873-1931)&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20231](http://rdaregistry.info/Elements/e/P20231)</td>
            <td>**workExpressed**</td>
            <td>&quot;Couperus, Louis (1863-19230) | Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20315](http://rdaregistry.info/Elements/e/P20315)</td>
            <td>**preferredTitleOfExpression**</td>
            <td>&quot;Am Wege der Freude&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20059](http://rdaregistry.info/Elements/e/P20059)</td>
            <td>**manifestationOfExpression**</td>
            <td>&quot;Am Wege der Freude | Ulstein | [1920] | volume&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20346](http://rdaregistry.info/Elements/e/P20346)</td>
            <td>**translatorPerson**</td>
            <td>&quot;Otten, Else (1873-1931)&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20006](http://rdaregistry.info/Elements/e/P20006)</td>
            <td>**languageOfExpression**</td>
            <td>&quot;German&quot;</td>
        </tr>
        <tr>
            <td>[rdae:P20001](http://rdaregistry.info/Elements/e/P20001)</td>
            <td>**contentType**</td>
            <td>&quot;text&quot;</td>
        </tr>
    </tbody>
</table>
</div>

### Manifestation

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdanl:Manifestation</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30004](http://rdaregistry.info/Elements/m/P30004)</td>
            <td>**identifierForManifestation**</td>
            <td>&quot;kob102&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30139](http://rdaregistry.info/Elements/m/P30139)</td>
            <td>**expressionManifested**</td>
            <td>&quot;Couperus, Louis (1863-1923) | &quot;Aan den weg der vreugde | text | Dutch&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30294](http://rdaregistry.info/Elements/m/P30294)</td>
            <td>**authorizedAccessPointForManifestation**</td>
            <td>&quot;Aan den weg der vreugde | L.J. Veen | [1908]</td>
            <td>volume&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30156](http://rdaregistry.info/Elements/m/P30156)</td>
            <td>**titleProper**</td>
            <td>&quot;Aan den weg der vreugde&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30105](http://rdaregistry.info/Elements/m/P30105)</td>
            <td>**statementOfResponsibilityRelatingToTitleProper**</td>
            <td>&quot;door Louis Couperus&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30109](http://rdaregistry.info/Elements/m/P30109)</td>
            <td>**manufactureStatement**</td>
            <td>&quot;Nijmegen : G.J. Thieme&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30175](http://rdaregistry.info/Elements/m/P30175)</td>
            <td>**nameOfManufacturer**</td>
            <td>&quot;G.J. Thieme&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30087](http://rdaregistry.info/Elements/m/P30087)</td>
            <td>**placeOfManufacture**</td>
            <td>&quot;Nijmegen&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30111](http://rdaregistry.info/Elements/m/P30111)</td>
            <td>**publicationStatement**</td>
            <td>&quot;Amsterdam : L.J. Veen, [1908]&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30176](http://rdaregistry.info/Elements/m/P30176)</td>
            <td>**nameOfPublisher**</td>
            <td>&quot;L.J. Veen&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30088](http://rdaregistry.info/Elements/m/P30088)</td>
            <td>**placeOfPublication**</td>
            <td>&quot;Amsterdam&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30011](http://rdaregistry.info/Elements/m/P30011)</td>
            <td>**dateOfPublication**</td>
            <td>&quot;[1908]&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30003](http://rdaregistry.info/Elements/m/P30003)</td>
            <td>**modeOfIssuance**</td>
            <td>&quot;single unit&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30182](http://rdaregistry.info/Elements/m/P30182)</td>
            <td>**extentOfManifestation**</td>
            <td>&quot;207 pagina&#39;s&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30169](http://rdaregistry.info/Elements/m/P30169)</td>
            <td>**dimensions**</td>
            <td>&quot;21 cm&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30001](http://rdaregistry.info/Elements/m/P30001)</td>
            <td>**carrierType**</td>
            <td>&quot;volume&quot;</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdam:P30002](http://rdaregistry.info/Elements/m/P30002)</td>
            <td>**mediaType**</td>
            <td>&quot;unmediated&quot;</td>
            <td></td>
        </tr>
    </tbody>
</table>
</div>

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdanl:Manifestation</td>
        </tr>
        <tr>
            <td>[rdam:P30004](http://rdaregistry.info/Elements/m/P30004)</td>
            <td>**identifierForManifestation**</td>
            <td>&quot;kob108&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30139](http://rdaregistry.info/Elements/m/P30139)</td>
            <td>**expressionManifested**</td>
            <td>&quot;Couperus, Louis (1863-1923) | Een vrouw van het noorden | text | Dutch&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30294](http://rdaregistry.info/Elements/m/P30294)</td>
            <td>**authorizedAccessPointForManifestation**</td>
            <td>&quot;Een vrouw van het noorden | Pandora | [1999] | volume | 2e dr&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30156](http://rdaregistry.info/Elements/m/P30156)</td>
            <td>**titleProper**</td>
            <td>&quot;Een vrouw van het noorden&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30128](http://rdaregistry.info/Elements/m/P30128)</td>
            <td>**variantTitleOfManifestation**</td>
            <td>&quot;Aan den weg der vreugde&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30105](http://rdaregistry.info/Elements/m/P30105)</td>
            <td>**statementOfResponsibilityRelatingToTitleProper**</td>
            <td>&quot;Louis Couperus&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30109](http://rdaregistry.info/Elements/m/P30109)</td>
            <td>**manufactureStatement**</td>
            <td>&quot;Nijmegen : G.J. Thieme&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30175](http://rdaregistry.info/Elements/m/P30175)</td>
            <td>**nameOfManufacturer**</td>
            <td>&quot;G.J. Thieme&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30087](http://rdaregistry.info/Elements/m/P30087)</td>
            <td>**placeOfManufacture**</td>
            <td>&quot;Nijmegen&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30111](http://rdaregistry.info/Elements/m/P30111)</td>
            <td>**publicationStatement**</td>
            <td>&quot;Amsterdam : L.J. Veen, [1908]&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30176](http://rdaregistry.info/Elements/m/P30176)</td>
            <td>**nameOfPublisher**</td>
            <td>&quot;L.J. Veen&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30088](http://rdaregistry.info/Elements/m/P30088)</td>
            <td>**placeOfPublication**</td>
            <td>&quot;Amsterdam&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30133](http://rdaregistry.info/Elements/m/P30133)</td>
            <td>**designationOfEdition**</td>
            <td>&quot;2e dr&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30011](http://rdaregistry.info/Elements/m/P30011)</td>
            <td>**dateOfPublication**</td>
            <td>&quot;[1908]&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30003](http://rdaregistry.info/Elements/m/P30003)</td>
            <td>**modeOfIssuance**</td>
            <td>&quot;single unit&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30182](http://rdaregistry.info/Elements/m/P30182)</td>
            <td>**extentOfManifestation**</td>
            <td>&quot;158 pagina&#39;s&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30169](http://rdaregistry.info/Elements/m/P30169)</td>
            <td>**dimensions**</td>
            <td>&quot;18 cm&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30001](http://rdaregistry.info/Elements/m/P30001)</td>
            <td>**carrierType**</td>
            <td>&quot;volume&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30002](http://rdaregistry.info/Elements/m/P30002)</td>
            <td>**mediaType**</td>
            <td>&quot;unmediated&quot;</td>
        </tr>
    </tbody>
</table>
</div>

<div class="example">
<table class='data'>
    <thead>
        <tr>
            <th>uri</th>
            <th>naam</th>
            <th>waarde</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>rdf:type</td>
            <td>**a**</td>
            <td>rdanl:Manifestation</td>
        </tr>
        <tr>
            <td>[rdam:P30004](http://rdaregistry.info/Elements/m/P30004)</td>
            <td>**identifierForManifestation**</td>
            <td>&quot;kob08&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30139](http://rdaregistry.info/Elements/m/P30139)</td>
            <td>**expressionManifested**</td>
            <td>&quot;Am Wegen der Freude | Ullstein | [1920] | volume&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30294](http://rdaregistry.info/Elements/m/P30294)</td>
            <td>**authorizedAccessPointForManifestation**</td>
            <td>&quot;Aan den weg der vreugde | L.J. Veen | [1908] | volume&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30156](http://rdaregistry.info/Elements/m/P30156)</td>
            <td>**titleProper**</td>
            <td>&quot;Am Wege der Freude&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30328](http://rdaregistry.info/Elements/m/P30328)</td>
            <td>**titleOfSeries**</td>
            <td>&quot;Ullstein-Bücher&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30105](http://rdaregistry.info/Elements/m/P30105)</td>
            <td>**statementOfResponsibilityRelatingToTitleProper**</td>
            <td>&quot;autor. Übertr. aus dem Holländischen von Else Otten&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30335](http://rdaregistry.info/Elements/m/P30335)</td>
            <td>**otherTitleInformation**</td>
            <td>&quot;Roman&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30111](http://rdaregistry.info/Elements/m/P30111)</td>
            <td>**publicationStatement**</td>
            <td>&quot;Amsterdam : L.J. Veen, [1908]&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30176](http://rdaregistry.info/Elements/m/P30176)</td>
            <td>**nameOfPublisher**</td>
            <td>&quot;Ullstein&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30088](http://rdaregistry.info/Elements/m/P30088)</td>
            <td>**placeOfPublication**</td>
            <td>&quot;Berlin&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30011](http://rdaregistry.info/Elements/m/P30011)</td>
            <td>**dateOfPublication**</td>
            <td>&quot;[1920]&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30003](http://rdaregistry.info/Elements/m/P30003)</td>
            <td>**modeOfIssuance**</td>
            <td>&quot;single unit&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30182](http://rdaregistry.info/Elements/m/P30182)</td>
            <td>**extentOfManifestation**</td>
            <td>&quot;278 pagina&#39;s&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30169](http://rdaregistry.info/Elements/m/P30169)</td>
            <td>**dimensions**</td>
            <td>&quot;15 cm&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30001](http://rdaregistry.info/Elements/m/P30001)</td>
            <td>**carrierType**</td>
            <td>&quot;volume&quot;</td>
        </tr>
        <tr>
            <td>[rdam:P30002](http://rdaregistry.info/Elements/m/P30002)</td>
            <td>**mediaType**</td>
            <td>&quot;unmediated&quot;</td>
        </tr>
    </tbody>
</table>
</div>