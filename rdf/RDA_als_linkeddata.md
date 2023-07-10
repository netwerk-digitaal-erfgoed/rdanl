RDA als linked data {#rda-als-ld}
=====================

Voor informatieprofessionals met een achtergrond in linked data en RDF, lijkt RDA op het eerste gezicht niets anders te zijn dan ‘gewoon’ een specialistisch RDF-vocabulaire gericht op het bibliotheekdomein. In de kern klopt dat, maar vaak is RDA anders opgezet dan je vanuit een gangbaar RDF-perspectief zou verwachten. Om RDA beter te kunnen doorgronden, en zo bijvoorbeeld spraakverwarring met collega’s te voorkomen, worden hier enige belangrijke verschillen met meer reguliere linked data-benaderingen behandeld.

RDA is in de huidige vorm vooral opgezet voor een wereld waarin het werken met bibliografische *records* centraal staat. De RDA-standaard biedt daarbij ook een **brug naar de toekomst** waarin linked data de norm is, zonder dat RDA zelf volledig op linked data-principes en -gebruiken gebaseerd is. Vanuit het linked data-perspectief zijn er binnen RDA keuzes gemaak die minder logisch of vaak zelf onhandig lijken. Ook de terminologie die binnen RDA gehanteerd wordt, lijkt vaak wel op die van RDF en linked data, maar heeft soms een in belangrijke mate verschillende betekenis.

## Lexical aliases
RDA komt uit een traditie waarin er veel aandacht is voor de waarde en het behoud van de verschillende wereldtalen. De classes en properties in RDA hebben daarom niet zoals gebruikelijk een makkelijk te onthouden ‘internationale,’ op de Engelse taal gebaseerde term zoals we kennen van **Dublin Core** of **Schema.org**, maar een abstracte naam, zoals `rdac:C10001` als aanduiding van een instantie behorende tot de `Work`-class of `rdaw:P10436` voor een kenmerk gelabeld met “*has author Person*”. Dit maakt menselijke interpretatie van RDA in RDF-vorm lastig. RDA biedt aanvullend wel zogenaamde *lexical aliases* in meerdere talen, zoals bijvoorbeeld [rdaa:contributorCollectiveAgentOfSpeechOf.en](http://rdaregistry.info/Elements/a/contributorCollectiveAgentOfSpeechOf.en). Deze functioneren echter niet zoals verwacht; als ze opgevraagd worden geven ze een http-error. Ook bieden ze geen `owl:equivalentClass`- of `owl:equivalentProperty`-relatie voor semantische inferentie. Ze zijn voor praktische toepassingen daarmee geen volwaardig equivalent voor de canonieke kenmerken en zouden in een RDF-context dan **vermeden moeten worden**. Vanwege de leesbaarheid zullen in deze tekst wel de lexical aliases gebruikt worden (overigens zonder de toevoeging van de taal-‘extensie’).

## Het begrip ‘range’ in RDA versus RDF
Binnen RDA, bijvoorbeeld in de [RDA Toolkit](https://www.rdatoolkit.org/), wordt van kenmerken (ofwel *properties*, binnen RDA meestal van elementen, deze term wordt ook aanduiding van de klassen gebruikt) vaak een ‘range’ aangeduid. Die *range* is dan zoals verwacht de klasse van het object waar het kenmerk naar verwijst. Dat klinkt als vergelijkbaar met het `rdfs:range`-kenmerk uit RDF, maar bij RDA wordt een ander abstractieniveau gehanteerd. Zo stelt RDA bijvoorbeeld dat de *range* van het kenmerk `rdaw:authorPerson` een `rdac:Person` is. Vanuit een RDF-perspectief lijkt de volgende *triple* dan incorrect, immers de `rdfs:range` is hier een `rdfs:Literal`, maar het volgende is binnen RDA als RDF helemaal correct::

<xmp highlight=turtle>
	<work_1> rdaw:authorPerson "Harry Mulisch" .
</xmp>

Halen we de definitie in RDF van de `rdaw:authorPerson` erbij, dan treffen we daar als `skos:definition` "*Relateert een werk aan een persoon die verantwoordelijk is voor het creëren van een tekstwerk.*" Echter, een `rdfs:range` wordt hier niet gedefinieerd. Waarom doet RDA dat niet? Wat RDA bedoelt met dat de range van `rdaw:authorPerson` een ‘Person’ is, is dat de voorgaande RDF als volgt herschreven kan worden:

<xmp highlight=turtle>
	<work_1> rdaw:authorPerson [
		a  rdac:Person ;
		rdaa:nameOfPerson "Harry Mulisch" 
	] .
</xmp>

RDA biedt zo voor toepassing in *record*-gebaseerde registratiesystemen een snelle manier om aan te kunnen geven dat een werk door een entiteit uit de klasse `rdac:Person` geschreven is, én dat “*Harry Mulisch*” een naam van die persoon is.

Enigszins terzijde: omdat de range van `rdaa:nameOfPerson` volgens RDA een `Nomen`-entiteit is, zou voorgaande RDF zelfs als volgt herschreven kunnen worden (maar deze aanpak heeft hier geen praktische meerwaarde):

<xmp highlight=turtle>
	<work_1> rdaw:authorPerson [
		a  rdac:Person ;
		rdaa:nameOfPerson [
			a rdac:Nomen ;
			rdan:nomenString "Harry Mulisch" 
		]
	] .
</xmp>

RDA biedt overigens ook twee andere sets met kenmerken waarin de `rdfs:range` *wel* gedefinieerd is. Kenmerken zoals `rdaw:authorPerson` bieden twee *subproperties*. De ene *subproperty*, `rdawd:authorPerson`, heeft als `rdfs:range` de `rdfs:Literal`(hoewel dit voor het 'data type'-kenmerk niet expliciet gebeurt, ie ook [issue #182](https://github.com/RDARegistry/RDA-Vocabularies/issues/182)). De andere *subproperty*, `rdawo:authorPerson`, heeft als `rdfs:range` de klasse `rdaw:Person`. RDA noemt deze *subproperties* respectievelijk de ‘data type’-*subproperty* en de ‘object type’-*subproperty*. Het bovenliggende kenmerk `rdaw:authorPerson` moet binnen RDA als canoniek beschouwd worden.

## Een veelheid aan beperkte kenmerken 
Een keerzijde van de voorgaand beschreven insteek van RDA, die efficiënt en noodzakelijk kan zijn voor het catalogiseren in een *records*-gebaseerd systeem, is dat er een veelheid aan kenmerken, ontstaat terwijl dat binnen een strikt RDF-perspectief semantisch niet noodzakelijk is. Dit speelt des te meer, aangezien RDA niet alleen een onderscheidende *range* als criterium voor het instellen van een kenmerk hanteert, maar ook een onderscheidend *domain*. Daar waar voor een strikte linked data-benadering met één kenmerk als bijvoorbeeld `related` zou kunnen worden volstaan, biedt RDA nu 169 varianten (RDA biedt 13 klassen, 13 x 13 = 169 mogelijke onderlinge relaties) van `related`-kennmerken, zoals bijvoorbeeld `rdaa:relatedCorporateBodyOfAgent`, `rdaa:relatedAgenOfPerson`, `rdaa:relatedFamilyOfPerson` of `rdaa:relatedCollectiveAgentOfAgent`,  *etcetera*. Bedenk daarbij dat ieder canonieke kenmerk ook een 'data type'- en een 'object type'-kenmerk heeft (maakt in totaal 13 x 13 x 3 = 507 mogelijk kenmerken, enkel om aan te geven dat twee entiteiten aan elkaar gerelateerd zijn) én dat van al die properties ook *lexical aliases* gedefinieerd zijn, in een veelheid aan talen.
Deze complexiteit van RDA is een reden waarom RDA als standaard niet zomaar ‘direct’ toe te passen is, maar waarom er vanuit een kaderend toepassingsprofiel gewerkt moet worden.
 
## Superelementen?
Binnen RDA wordt in de context van een kenmerk soms gesproken over een *superelement*. Dit schept het beeld van twee kenmerken die in relatie tot elkaar staan als:

<xmp highlight=turtle>
	:element rdfs:subPropertyOf :superelement .
</xmp>

Dat is een **onjuiste aanname**. RDA doelt hier niet op een hiërarchische relatie. Een superelement is in RDA een kenmerk dat op *aggregerende* wijze gevens uit andere kenmerken overneemt.
 
 
## Wel RDF, nog geen linked data
Beschrijvingen in RDA kunnen één-op-één weggeschreven worden als RDF *triples*. Maakt dit RDA ook tot linked data? Niet per se! Een basisprincipe achter linked data is dat de onderscheiden entiteiten van een IRI (van oudsher ook wel URI genoemd, een IRI is speciek een URI die ook geschikt is voor niet-ASCII tekens) te voorzien en die IRI dan in verwijzingen als **representatie** voor die entiteit te gebruiken. In RDA worden echter nadrukkelijk ook andere methoden toegestaan om naar entiteiten te verwijzen. RDA spreekt daarbij van **implementatie-scenario’s**. Een gangbaar implementatie-scenario uit de wereld van *records*-gebaseerd catalogiseren is het gebruik van *geautoriseerde ingangen* (‘*authorized access points*’). Een geautoriseerde ingang is een binnen het betreffende domein unieke *identifier* voor een entiteit in een gestructureerde, en voor mensen leesbare en begrijpelijke vorm. Voor bijvoorbeeld de schrijver “*Harry Mulisch*” zou zo’n ingang  “*Mulisch, Harry (1927 – 2010)*” kunnen zijn.

Duidelijk is dat we in een linked data-toepassing IRI’s, in plaats van geautoriseerde ingangen, zouden willen gebruiken om entiteiten te verbinden. Echter, als we geautoriseerde ingang hierbij achteloos vervangen door een IRI, dan zal dat leiden tot ongewenst informatieverlies. Een ingang is namelijk niet zomaar een *identifier*, maar een **betekenisdragende** *identifier*.
Dit probleem wordt zichtbaar in de casus van een schrijver die zich van meerdere namen bedient bij het uitbrengen van een werk. Graag komen we hierbij tegemoet aan de gebruikerswens van koningin Victoria:

Toen koningin Victoria vroeg om alle werken van de auteur van "*Alice in Wonderland*" kreeg ze tot haar verrassing ook een stapel wiskundige werken. Victoria was enkel geïnteresseerd in werken van Lewis Carroll, maar realiseerde zich niet dat het een pseudoniem is van de wiskundige Charles Lutwidge Dodgson. Deze koninklijke gebruikerswens kan door RDA gebaseerd op geautoriseerde ingangen goed vervuld worden. Stel onderstaande RDF voor:

<xmp highlight=turtle>
	<work_1>
		rdaw:authorPerson “Carroll, Lewis” .

	<work_2>
		rdaw:authorPerson “Dodgson, Charles Lutwidge” .

	<person_1>
		rdaa:authorizedAccessPointOfPerson “Dodgson, Charles Lutwidge” ;
		rdaa:authorizedAccessPointOfPerson “Carroll, Lewis” .
</xmp>

Hieruit zou, in lijn met de gebruikerswens, opgemaakt kunnen worden dat `<person_1>` de auteur is van `<work_1>` én van `<work_2>` maar dat alleen `<work_1>` bekend werd als publicatie onder de auteursnaam "*Lewis Carroll*". 

Als we nu de geautoriseerde ingangen vervangen door IRI’s, dan wordt duidelijk dat we de semantische waarde van deze ingangen missen. We weten dan niet meer welk werk behoort bij "*Lewis Carroll*".

<xmp highlight=turtle>
	<work_1>
		rdaw:authorPerson <person_1> .	# range is een Person

	<work_2>
		rdaw:authorPerson <person_1> . # range is een Person

	<person_1>
		rdaa:authorizedAccessPointOfPerson “Dodgson, Charles Lutwidge” ;
		rdaa:authorizedAccessPointOfPerson “Carroll, Lewis” .
</xmp>

Een linked data-gebaseerde oplossing voor deze gebruikerswens is te vinden in [Introductie van de Persona binnen RDA](#persona-in-rda).
