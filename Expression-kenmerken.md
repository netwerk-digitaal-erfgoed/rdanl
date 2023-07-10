Toe te passen RDA-kenmerken voor Expression-entiteiten {#item-kenmerken}
--------------------

Zie ook overzicht [RDA-kenmerken](RDA-kenmerken.md).


| uri | naam | opm. | range | vastlegging [^1] | verpl.? [^2] | max. | waarde |
| --- | --- | --- | --- | --- | --- | --- | --- |
||
|| *Appellation:* | *elementen om de entiteit te benoemen:* ||| M | >1 ||
| [rdae:P20312](http://rdaregistry.info/Elements/e/P20312) | **titleOfExpression** || `Nomen` | U | MA | 1 |
| [rdae:P20002](http://rdaregistry.info/Elements/e/P20002) | **identifierForExpression** | niet bedoeld voor de IRI van de entiteit zelf | `Nomen`	| identifier/iri	| MA | >1 ||
||
|| *Coherence*:	|*primaire relaties tussen entiteiten:* ||| M |
| [rdae:P20231](http://rdaregistry.info/Elements/e/P20231) | **workExpressed** || `Work` | S / Id / IRI | M | 1 |
| [rdae:P20059](http://rdaregistry.info/Elements/2/P20059) | **manifestationOfExpression** | relateer `Manifestations` aan de `Expression` vooral via de `Manifestation` | `Manifestation` | S / Id / IRI | O | >1 |
||
||	*General description:*	| *algemene beschrijving (basistoepassingsprofiel):* |
| [rdae:P20001](http://rdaregistry.info/Elements/e/P20001) | **contentType** || - | S / IRI | M | >1 | RDA Content Type [^3] |
| [rdae:P20006](http://rdaregistry.info/Elements/e/P20006) | **languageOfExpression** ||| S | M | >1 | ISO 639.2 |
| [rdae:P20071](http://rdaregistry.info/Elements/e/P20071) | **noteOnExpression** ||| U | O | >1 |
| [rdae:P20069](http://rdaregistry.info/Elements/e/P20069) | **summarizationOfContent** ||| U | O | >1 |
||
||	*General relationships:* | *algemene elementen om relaties van de entiteit te beschrijven (basistoepassingsprofiel):* |
| [rdae:P20214](http://rdaregistry.info/Elements/e/P20214) | **dateOfExpression** || `Timespan` | U / S / Id / IRI | MA | 1 | ISO 8601-1:2019 |
| [rdae:P20053](http://rdaregistry.info/Elements/e/P20053) | **creatorAgentOfExpression** | gebruik een zo specifiek mogelijke narrow element | `Agent` | S / Id / IRI | MA | >1 | NTA, NACO, Corporatiethesaurus |
| [rdae:P20325](http://rdaregistry.info/Elements/e/P20325) | **representativeExpressionOf** | gebruik dit element in ieder geval voor de Expression van de eerste Manifestation van het Work als meerdere Expressions aanwezig zijn | `Work` | S / Id / IRI | O | 1 |
| [rdae:P20205](http://rdaregistry.info/Elements/e/P20205) | **relatedExpressionOfExpression** | gebruik een zo specifiek mogelijk subelement, oa. voor vertalingen en bewerkingen | `Expression` | S / Id / IRI | MA | >1 |
||
||	*Special description:* | *Gespecialiseerde elementen om de entiteit te beschrijven:* |
| [rdae:P20322](http://rdaregistry.info/Elements/e/P20322) | **intendedAudienceOfExpression** ||| U / S / Id / IRI || MA | >1 || gebruik zoveel mogelijk een gecontroleerde waardelijst |
| [rdae:P20219](http://rdaregistry.info/Elements/e/P20219) | **duration** | voor gebruik bij luisterboeken || S || MA | 1 | ISO 8601-1:2019 |

[^1]: Vastlegging / *Recording method*, volgens <br>**U**: "unstructured"<br>**S**: "structured"<br>**Id**: "identifier" <br>**IRI**: IRI.
[^2]: Verplicht veld?, volgens <br>**M**: "*Must* / Verplicht"<br>**MA**: "*Must if applicable* / Verplicht indien van toepassing"<br>**O**: "*Optional* / Optioneel" 
[^3]: Zie [RDA Content Type](http://www.rdaregistry.info/termList/RDAContentType/?language=nl).
[^4]: Gebruik van subkenmerken met een specifiekere *range* helpt om in *records*-gebaseerde systemen de klasse van het object expliciet te maken. In een linked data-omgeving wordt juist aangeraden om zo algemeen mogelijke kenmerken te gebruiken én de RDF-entiteiten expliciet van een klasse te voorzien.