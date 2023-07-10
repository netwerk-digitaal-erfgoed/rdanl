**Deze repository is gearchiveerd en leeft verder op [http://github.com/netwerk-digitaal-erfgoed/rdanl](http://github.com/netwerk-digitaal-erfgoed/rdanl).**

# RDA-Toepassingsprofiel


Om bibliografische beschrijvingen van het **tijdperk van de kaartenbak** naar dat van **linked data** te brengen, en zo een **breed scala aan gebruikerswensen** te kunnen ondersteunen, daar is een nieuw fundament voor nodig. De catalogiseerstandaard **RDA** (*Resource Description and Access* [^1]) en daarmee het onderliggende conceptuele model **IFLA LRM** (IFLA Library Reference Model [^2]), biedt dit.

RDA heeft een grote uitdrukkingskracht, is flexibel, en toepasbaar in traditonele catalogiseersystemen én in linked data-voorzieningen. Een keerzijde hiervan is een hoge complexiteit. Om RDA in te kunnen zetten is daarom doorgaans een **toepassingsprofiel** onmisbaar. Een toepassingsprofiel vereenvoudigt de implementatie binnen een specifiek domein, door het bieden van **een passende selectie van elementen uit de standaard**, voorzien van **implementatie-voorbeelden**, **aanvullende richtlijnen** en **uitleg**.
 
Dat is wat ook dit RDA-toepassingsprofiel biedt. De horizon is het gebruik voor het beschrijven van de **Nederlandse bibliografie**, in deze fase nog beperkt tot monografieën, waaronder ook luisterboeken (zie [Scope toepassingsprofiel](Scope_toepassingsprofiel.md)).

Dit profiel richt zich op een **brede groep gebruikers**. Van catalografen in tradtionele, op *records*-gebaseerde catalogiseersystemen, die als eerste stap metadata willen verrijken om **RDA-entiteiten herkenbaar** te kunnen maken, via metadata-specialisten, die **systemen op RDA willen aansluiten**, tot aan ontwikkelaars uit de wereld van **linked data-gebaseerde integratievoorzieningen**.

## Leeswijzer

### De eerste stap naar RDA, vanuit bestaande systemen

* [Inleiding op RDA en IFLA LRM](RDA_en_LRM.md): wat is RDA en hoe verhoudt het zich tot IFLA LRM?
* [Van 'legacy'-metadata naar RDA-entiteiten](Van_legacy-metadata_naar_RDA-entiteiten.md): een **stappenplan** gebaseerd op een lijst met **minimale metadata-eisen**.

### Verdere integratie van RDA in catalogiseersystemen

* [Toe te passen RDA-kenmerken](RDA-kenmerken.md): Overzicht toe te passen RDA-kenmerken, per soort entiteit.
* [Introductie van de 'Persona' binnen RDA](Persona_in_RDA.md): Modellering van **publieke identiteiten** ('Personae') van schrijvers binnen de kaders van RDA.

### RDA in linked data-toepassingen 

* [RDA als linked data](rdf/RDA_als_linkeddata.md): Wat een informatieprofessional met een achtergrond in RDF moet weten over RDA.
* [Toepassingsprofiel RDANL in RDF](rdf/profile): Een toepassingsprofiel voor RDA als **ontologie in RDF**, vooral gericht op linked data-toepassingen.
* [Voorbeelden van RDA in RDF](rdf/examples): **Voorbeelden in RDF** van bibliografische beschrijvingen en van een uitwerking van de modellering van *Personae*. 
 
## Afsluitend

Dit RDA-toepassingsprofiel is opgesteld door Sita Bhagwandin, Djoke Dam,  Meta van der Waal-Gentenaar, René Voorburg en Brigitte den Oudsten van de [KB | nationale bibliotheek](https://www.kb.nl/), in opdracht van [Netwerk Digitaal Erfgoed](https://netwerkdigitaalerfgoed.nl) en met financiële steun uit programmalijn '[Verbonden Digitaal Erfgoed](https://www.stichtingpica.nl/programmalijnen/verbonden-digitaal-erfgoed/)' van de [Stichting PICA](https://www.stichtingpica.nl/).


[^1]: RDA wordt beheerd door de [RDA Steering Committee](http://www.rda-rsc.org)
[^2]: Zie [IFLA Library Reference Model: A Conceptual Model for Bibliographic Information](https://repository.ifla.org/handle/123456789/40)
