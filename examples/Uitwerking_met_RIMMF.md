# Uitwerking met RIMMF


*Ter illustratie* de volgende beschrijving van een `Work` met bijbehorende `Expressions` en `Manifestations` zoals gegeneerd door RIMMF [^1]. Hierbij wordt een traditioneel implementatiescenario gevolgd, gebaseerd op (geautoriseerde) ingangen. De identifiers zijn door RIMMF gegeneerd. 

In dit voorbeeld van RIMMF wordt niet de voorgestelde [Persona-aanpak](Persona_in_RDA.md) gevolgd, of de voorgestelde gestructureerde tekenreeksen (SES). Zie de [uitwerking in RDF](../rdf/examples) voor een beschrijving in lijn met de voorgestelde aanpak.



## Work

| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type| **a**	| rdac:Work |
| [rdaw:P10002](http://rdaregistry.info/Elements/w/P10002) | **identifierForWork** | "kob105" |
| [rdaw:P10223](http://rdaregistry.info/Elements/w/P10223) | **preferredTitleOfWork** | "Aan den weg der vreugde" |
| [rdaw:P10086](http://rdaregistry.info/Elements/w/P10086) | **variantTitleOfWork** | "Een vrouw van het noorden" |
| [rdaw:P10331](http://rdaregistry.info/Elements/w/P10331) | **authorizedAccessPointForWork** | "Couperus, Louis (1863-1923 \| Aan den weg der vreugde" |
| [rdaw:P10332](http://rdaregistry.info/Elements/w/P10332) | **variantAccessPointForWork** | "Couperus, Louis (1863-1923 \| Een vrouw van het noorden" |
| [rdaw:P10004](http://rdaregistry.info/Elements/w/P10004) | **categoryOfWork** | "romans en novellen" |
| [rdaw:P10365](http://rdaregistry.info/Elements/w/P10365) | **extensionPlan** | "static plan" |
| [rdaw:P10078](http://rdaregistry.info/Elements/w/P10078) | **expressionOfWork** | "Couperus, Louis (1863-1923) \| Aan den weg der vreugde \| text \| Dutch" |
| [rdaw:P10436](http://rdaregistry.info/Elements/w/P10436) | **authorPerson** | "Couperus, Louis (1863-1923)" |
| [rdaw:P10219](http://rdaregistry.info/Elements/w/P10219) | **dateOfWork** | "1908" |


## Expression



| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type | **a**	| rdanl:Expression |
| [rdae:P20002](http://rdaregistry.info/Elements/e/P20002) | **identifierForExpression** | "kob103" |
| [rdae:P20313](http://rdaregistry.info/Elements/e/P20313) | **authorizedAccessPointForExpression** | "Couperus, Louis (1863-1923) \| Aan den weg der vreugde \| text \| Dutch" |
| [rdae:P20231](http://rdaregistry.info/Elements/e/P20231) | **workExpressed** | "Couperus, Louis (1863-1923 \| Aan den weg der vreugde" |
| [rdae:P20059](http://rdaregistry.info/Elements/e/P20059) | **manifestationOfExpression** | "Aan den weg der vreugde \| L.J. Veen \| [1908] \| volume " |
| [rdae:P20006](http://rdaregistry.info/Elements/e/P20006) | **languageOfExpression** | "Dutch" |
| [rdae:P20001](http://rdaregistry.info/Elements/e/P20001) | **contentType** | "text" |

| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type | **a**	| rdanl:Expression |
| [rdae:P20002](http://rdaregistry.info/Elements/e/P20002) | **identifierForExpression** | "kob109" |
| [rdae:P20313](http://rdaregistry.info/Elements/e/P20313) | **authorizedAccessPointForExpression** | "Couperus, Louis (1863-1923) \| Een vrouw van het noorden \| text \| Dutch" |
| [rdae:P20231](http://rdaregistry.info/Elements/e/P20231) | **workExpressed** | "Couperus, Louis (1863-1923 \| Aan den weg der vreugde" |
| [rdae:P20315](http://rdaregistry.info/Elements/e/P20315) | **preferredTitleOfExpression** | "Een vrouw van het noorden" |
| [rdae:P20059](http://rdaregistry.info/Elements/e/P20059) | **manifestationOfExpression** | "Een vrouw van het noorden \| Pandorra \| [1999] \| volume \| 2e dr" |
| [rdae:P20006](http://rdaregistry.info/Elements/e/P20006) | **languageOfExpression** | "Dutch" |
| [rdae:P20001](http://rdaregistry.info/Elements/e/P20001) | **contentType** |  "text" |

| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type | **a**	| rdanl:Expression |
| [rdae:P20002](http://rdaregistry.info/Elements/e/P20002) | **identifierForExpression** | "kob111" |
| [rdae:P20313](http://rdaregistry.info/Elements/e/P20313) | **authorizedAccessPointForExpression** | "Am Wege der Freude \| text \| German \| Otten, Else (1873-1931)"  |
| [rdae:P20231](http://rdaregistry.info/Elements/e/P20231) | **workExpressed** |"Couperus, Louis (1863-1923 \| Aan den weg der vreugde" |
| [rdae:P20315](http://rdaregistry.info/Elements/e/P20315) | **preferredTitleOfExpression** |  "Am Wege der Freude" |
| [rdae:P20059](http://rdaregistry.info/Elements/e/P20059) | **manifestationOfExpression** | "Am Wege der Freude \| Ulstein \| [1920] \| volume" |
| [rdae:P20346](http://rdaregistry.info/Elements/e/P20346) | **translatorPerson** | "Otten, Else (1873-1931)" |
| [rdae:P20006](http://rdaregistry.info/Elements/e/P20006) | **languageOfExpression** | "German" |
| [rdae:P20001](http://rdaregistry.info/Elements/e/P20001) | **contentType** |  "text" |

## Manifestation

| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type | **a**	| rdanl:Manifestation |
| [rdam:P30004](http://rdaregistry.info/Elements/m/P30004) | **identifierForManifestation** | "kob102" |
| [rdam:P30139](http://rdaregistry.info/Elements/m/P30139) | **expressionManifested** |  "Couperus, Louis (1863-1923) \| "Aan den weg der vreugde \| text \| Dutch" |
| [rdam:P30294](http://rdaregistry.info/Elements/m/P30294) | **authorizedAccessPointForManifestation** | "Aan den weg der vreugde \| L.J. Veen \| [1908] | volume" |
| [rdam:P30156](http://rdaregistry.info/Elements/m/P30156) | **titleProper** |  "Aan den weg der vreugde" |
| [rdam:P30105](http://rdaregistry.info/Elements/m/P30105) | **statementOfResponsibilityRelatingToTitleProper** | "door Louis Couperus" | 
| [rdam:P30109](http://rdaregistry.info/Elements/m/P30109) | **manufactureStatement** |  "Nijmegen : G.J. Thieme" |
| [rdam:P30175](http://rdaregistry.info/Elements/m/P30175) | **nameOfManufacturer** |  "G.J. Thieme" | 
| [rdam:P30087](http://rdaregistry.info/Elements/m/P30087) | **placeOfManufacture** | "Nijmegen" |
| [rdam:P30111](http://rdaregistry.info/Elements/m/P30111) | **publicationStatement** |  "Amsterdam : L.J. Veen, [1908]" |
| [rdam:P30176](http://rdaregistry.info/Elements/m/P30176) | **nameOfPublisher** | "L.J. Veen" |
| [rdam:P30088](http://rdaregistry.info/Elements/m/P30088) | **placeOfPublication** | "Amsterdam" |
| [rdam:P30011](http://rdaregistry.info/Elements/m/P30011) | **dateOfPublication** | "[1908]" |
| [rdam:P30003](http://rdaregistry.info/Elements/m/P30003) | **modeOfIssuance** | "single unit" | 
| [rdam:P30182](http://rdaregistry.info/Elements/m/P30182) | **extentOfManifestation** | "207 pagina's" |
| [rdam:P30169](http://rdaregistry.info/Elements/m/P30169) | **dimensions** | "21 cm" |
| [rdam:P30001](http://rdaregistry.info/Elements/m/P30001) | **carrierType** | "volume" |
| [rdam:P30002](http://rdaregistry.info/Elements/m/P30002) | **mediaType** | "unmediated" |

| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type | **a**	| rdanl:Manifestation |
| [rdam:P30004](http://rdaregistry.info/Elements/m/P30004) | **identifierForManifestation** | "kob108" |
| [rdam:P30139](http://rdaregistry.info/Elements/m/P30139) | **expressionManifested** | "Couperus, Louis (1863-1923) \| Een vrouw van het noorden \| text \| Dutch" |
| [rdam:P30294](http://rdaregistry.info/Elements/m/P30294) | **authorizedAccessPointForManifestation** | "Een vrouw van het noorden \| Pandora \| [1999] \| volume \| 2e dr" |
| [rdam:P30156](http://rdaregistry.info/Elements/m/P30156) | **titleProper** | "Een vrouw van het noorden" |
| [rdam:P30128](http://rdaregistry.info/Elements/m/P30128) | **variantTitleOfManifestation** | "Aan den weg der vreugde" |
| [rdam:P30105](http://rdaregistry.info/Elements/m/P30105) | **statementOfResponsibilityRelatingToTitleProper** |  "Louis Couperus" | 
| [rdam:P30109](http://rdaregistry.info/Elements/m/P30109) | **manufactureStatement** | "Nijmegen : G.J. Thieme" |
| [rdam:P30175](http://rdaregistry.info/Elements/m/P30175) | **nameOfManufacturer** | "G.J. Thieme" | 
| [rdam:P30087](http://rdaregistry.info/Elements/m/P30087) | **placeOfManufacture** | "Nijmegen" |
| [rdam:P30111](http://rdaregistry.info/Elements/m/P30111) | **publicationStatement** | "Amsterdam : L.J. Veen, [1908]" |
| [rdam:P30176](http://rdaregistry.info/Elements/m/P30176) | **nameOfPublisher** | "L.J. Veen" |
| [rdam:P30088](http://rdaregistry.info/Elements/m/P30088) | **placeOfPublication** | "Amsterdam" |
| [rdam:P30133](http://rdaregistry.info/Elements/m/P30133) | **designationOfEdition** | "2e dr" |
| [rdam:P30011](http://rdaregistry.info/Elements/m/P30011) | **dateOfPublication** | "[1908]" |
| [rdam:P30003](http://rdaregistry.info/Elements/m/P30003) | **modeOfIssuance** | "single unit" | 
| [rdam:P30182](http://rdaregistry.info/Elements/m/P30182) | **extentOfManifestation** |"158 pagina's" |
| [rdam:P30169](http://rdaregistry.info/Elements/m/P30169) | **dimensions** | "18 cm" |
| [rdam:P30001](http://rdaregistry.info/Elements/m/P30001) | **carrierType** | "volume" |
| [rdam:P30002](http://rdaregistry.info/Elements/m/P30002) | **mediaType** | "unmediated" |


| uri | naam | waarde |
| --- | --- | --- |
| rdfs:type | **a**	| rdanl:Manifestation |
| [rdam:P30004](http://rdaregistry.info/Elements/m/P30004) | **identifierForManifestation** | "kob08" |
| [rdam:P30139](http://rdaregistry.info/Elements/m/P30139) | **expressionManifested** |  "Am Wegen der Freude \| Ullstein \| [1920] \| volume" |
| [rdam:P30294](http://rdaregistry.info/Elements/m/P30294) | **authorizedAccessPointForManifestation** | "Aan den weg der vreugde \| L.J. Veen \| [1908] \| volume" |
| [rdam:P30156](http://rdaregistry.info/Elements/m/P30156) | **titleProper** |  "Am Wege der Freude" |
| [rdam:P30328](http://rdaregistry.info/Elements/m/P30328) | **titleOfSeries** | "Ullstein-Bücher" |
| [rdam:P30105](http://rdaregistry.info/Elements/m/P30105) | **statementOfResponsibilityRelatingToTitleProper** | "autor. Übertr. aus dem Holländischen von Else Otten" | 
| [rdam:P30335](http://rdaregistry.info/Elements/m/P30335) | **otherTitleInformation** | "Roman" |
| [rdam:P30111](http://rdaregistry.info/Elements/m/P30111) | **publicationStatement** |  "Amsterdam : L.J. Veen, [1908]" |
| [rdam:P30176](http://rdaregistry.info/Elements/m/P30176) | **nameOfPublisher** | "Ullstein" |
| [rdam:P30088](http://rdaregistry.info/Elements/m/P30088) | **placeOfPublication** |  "Berlin" |
| [rdam:P30011](http://rdaregistry.info/Elements/m/P30011) | **dateOfPublication** | "[1920]" |
| [rdam:P30003](http://rdaregistry.info/Elements/m/P30003) | **modeOfIssuance** | "single unit" | 
| [rdam:P30182](http://rdaregistry.info/Elements/m/P30182) | **extentOfManifestation** | "278 pagina's" |
| [rdam:P30169](http://rdaregistry.info/Elements/m/P30169) | **dimensions** | "15 cm" |
| [rdam:P30001](http://rdaregistry.info/Elements/m/P30001) | **carrierType** | "volume" |
| [rdam:P30002](http://rdaregistry.info/Elements/m/P30002) | **mediaType** | "unmediated" |


[^1]: \[RIMMF](https://www.rimmf.com/) - RDA in Many Metadata Formats" - is een hulpmiddel voor MS Windows voor het (leren) werken met RDA.