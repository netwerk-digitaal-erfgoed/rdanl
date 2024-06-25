Voorbeelden RDA als RDF {#examples}
=============

Uitwerking van de modellering van Personae in RDA {#examples-personae}
-------------

<pre class=include-code>
path: rdf/examples/personae_rdanl.ttl
highlight: turtle
</pre>

Uitwerkingen Een vrouw van het noorden (Louis Couperus) {#examples-louis-couperus}
-------------

Een beschrijving in RDA van een `Manifestation` de bijbehorende `Expression`, `Work`, `Person` en *Persona* van "*Een vrouw van het noorden*" van Louis Couperus. 

<pre class=include-code>
path: rdf/examples/example_rda.ttl
highlight: turtle
</pre>

Dezelfde entiteiten worden op semantisch identieke wijze beschreven, maar dan gebruikmakend van de afgeleide klasses en kenmerken zoals gedefinieerd in het toepassingsprofiel.

<pre class=include-code>
path: rdf/examples/personae_rdanl.ttl
highlight: turtle
</pre>

Ter vergelijking is het voorbeeld in het schema.org-vocabulaire uitgewerkt. Dit op basis van het [LRM to schema.org-toepassingsprofiel](http://data.bibliotheken.nl/files/LRM2schema.pdf).

<pre class=include-code>
path: rdf/examples/example_schema.ttl
highlight: turtle
</pre>

## Gevolgde principes
De voorbeeld-RDF van "*Een vrouw van het noorden*" is op de volgende principes gebaseerd:

* Informatie-eenheden worden zo veel mogelijk als een RDA/RDF-entiteit gedefinieerd, met uitzondering van `Nomens` en `Timespans`. Deze laatste worden standaard als `rdfs:Literal` opgenomen, tenzij er semantische noodzaak is ze toch als entiteit op te nemen.
* Alle entiteiten worden expliciet van een klasse-aanduiding voorzien. Dit verhoogt de begrijpelijkheid van de RDF én maakt het mogelijk om generieke relaties toe te passen.
* De kenmerken worden zo generiek mogelijk gekozen. Doordat alle entiteiten van  een klasse-aanduiding voorzien zijn, doet dit geen afbraak aan de semantische rijkdom. Het bevragen van de data, bijvoorbeeld met SPARQL, wordt hierdoor ook vereenvoudigd.
* Voor taalcodes wordt [IETF BCP 47](https://www.rfc-editor.org/info/bcp47) gebruikt. Het gebruik van URI’s boven literals heeft hier geen meerwaarde.
* Op vergelijkbare wijze is voor landencodes gebruik gemaakt van literals volgens [ISO 3166-1 alpha-2](https://nl.wikipedia.org/wiki/ISO_3166-1_alpha-2) .
* `Timespans` worden ingevuld als literals volgens [ISO 8601](https://nl.wikipedia.org/wiki/ISO_8601), zonder een datatype-aanduiding.
* Bij de `placeOfPublication` wordt een geneste constructie gebruikt, om zo plaatsnaam en land met elkaar te kunnen verbinden.
* De RDF wordt opgebouwd volgens de [modellering van Personae in RDA](#persona-in-rda).
* Kenmerken als `languageOfRepresentativeExpression` worden op het meest specifieke niveau aangeduid, dus in dit voorbeeld als eigenschap van het object van `representatieveExpression`, niet als eigenschap van het `Work` (wat uiteraard alleen mogelijk is als er ook een `representativeExpression` aangewezen kan worden).

De volgende kleurcodering wordt er in de voorbeelden gebruikt:

🟩Work🟩

🟦Expression🟦

🟨Manifestation🟨

🟥Item🟥 