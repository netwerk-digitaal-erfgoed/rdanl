# Toepassingsprofiel rdanl in RDF

Toepassingsprofiel `rdanl` is een op RDA gebaseerde ontologie in RDF-vorm. Het is gericht op het verlagen van de toegang tot RDA door het bieden van een wat beknoptere set met **kernelementen**, in een **voor mensen leesbare vorm**. De toepassing is bovenal, maar niet uitsluitend, voor linked data-omgevingen.

Het toepassingsprofiel `rdanl` biedt in RDF-vorm: 

* alle klassen en kernmerken zoals expliciet benoemd in het [RDA-toepassingsprofiel](#rda-kenmerken),
* aanvullende (rol-) kenmerken gebaseerd op een analyse van rollen gebruikt bij de beschrijving van de Nederlandse romans in het GGC,
* aanvullende (rol-) kenmerken waarbij de *range* een `Agent` is.

Deze laatste groep kenmerken is toevoegd om zo de semantische rijkdom van RDA te kunnen bieden bij RDF-toepassingen. Het principe hier achter is dat de veelheid van naar *range* en *domain* gedifferentieerde kenmerken die RDA biedt, geen semantische meerwaarde oplevert in een context waarbij alle entiteiten expliciet van een klasse-aanduiding voorzien zijn. Onder deze voorwaarde wordt een groot deel van de kenmerken van RDA overbodig en kan zo deze ontologie relatief beperkt blijven (deze ontologie biedt ~ 400 elementen).

Dit profiel in RDF is minder uitgebreid dan RDA, maar omdat het een **extensie van RDA** is, kan het waar nodig, gecombineerd worden met elementen uit RDA zelf.

Bovendien biedt deze ontologie URI's voor de elementen die zowel voor machnines als **voor mensen leesbaar** zijn. De URI's zijn daarbij gebaseerd op de Engelstalige *lexical aliasses* van RDA. De bestaande *lexical aliasses* van RDA zijn wel voor mensen leesbaar, maar niet, of beperkt, machine-leesbaar omdat ze zich niet aan gangbare linked data-principes conformeren.

## rdanl in meer detail

* De URI's van `rdanl` zijn uit het oogpunt van gebruiksgemak gedefinieerd binnen één *namespace*, te weten  `http://data.bibliotheken.nl/rdanl#`, bij voorkeur te gebruiken met als *namespace prefix* `rdanl`.
* Klasses binnen `rdanl` zijn gedefinieerd als een `owl:sameAs` van de overeenkomstige klasse in RDA.
* Kenmerken zijn in `rdanl` gedefinieerd als een `owl:sameAs` van het overeenkomstige kenmerk in RDA.
* Als verbijzondering van een RDA-toepassingsprofiel voor monografieën *kunnen* kenmerken relevant voor andere materiaalsoorten ontbreken.
* Ter ondersteuning van de [Persona-modellering](#persona-in-rda) is kenmerk `rdanl:relatedPersonaOfWork` toegevoegd, een `rdfs:subPropertyOf` van `rdanl:relatedNomenOfWork`. 
* Een kracht van RDA is de grote rijkdom aan kenmerken die **rollen** aanduiden. Vanuit de genoemde vereenvoudigingsprincipes is er een voorkeur voor rollen die betrekking hebben op instanties van de `rdanl:Agent`-klasse.
* De hierarchie in kenmerken binnen `rdanl` volgt impliciet die van RDA (via de `rdfs:subPropertyOf`-relatie). Uit *oogpunt van leesbaarheid* zijn deze relaties waar zinvol geacht ook expliciet in deze ontologie opgenomen.

## rdanl.ttl

<pre class=include-code>
path: rdf/profile/rdanl.ttl
highlight: turtle
</pre>
