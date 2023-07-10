Toe te passen RDA-kenmerken voor Item-entiteiten {#item-kenmerken}
--------------------

Zie ook overzicht [RDA-kenmerken](RDA-kenmerken.md).

| uri | naam | opm. | range | vastlegging [^1] | verpl.? [^2] | max. | waarde |
| --- | --- | --- | --- | --- | --- | --- | --- |
||
|| *Appellation:* | *elementen om de entiteit te benoemen:* ||| M | >1 |
| [rdai:P40001](http://rdaregistry.info/Elements/i/P40001) | **identifierForItem** || `Nomen` | Id | M | 1 | barcode, URN |
||
|| *Coherence:* | *primaire relaties tussen entiteiten:* ||| M | >1 |
| [rdai:P40049](http://rdaregistry.info/Elements/i/P40049) | **manifestationExemplified** || `Manifestation` | S / Id / IRI | M | 1 |
||
||	*General description:*	| *algemene beschrijving (basistoepassingsprofiel):* |
| [rdai:P40028](http://rdaregistry.info/Elements/i/P40028) | **noteOnItem** | voor het signatuur heeft RDA geen element, daarom kan indien gewenst het signatuur in edit met voorlooptekst "Signatuur:" opgenomen worden || U | O | >1 |
| [rdai:P40048](http://rdaregistry.info/Elements/i/P40048) | **restrictionOnUseOfItem** ||| U / S / Id / IRI | MA | 1 |
| [rdai:P40096](http://rdaregistry.info/Elements/i/P40096) | **categoryOfItem** ||| U / S / Id / IRI | O | 1 |
||
|| *General relationships:* | *algemene elementen om relaties van de entiteit te beschrijven (basistoepassingsprofiel):* |
| [rdai:P40162](http://rdaregistry.info/Elements/i/P40162) | **locationOfItem** || `Place` | S | M | 1 |
| [rdai:P40136](http://rdaregistry.info/Elements/i/P40136) | **ownerCorporateBody** || `CorporateBody` | S / Id / IRI | M | 1 |
| [rdai:P40046](http://rdaregistry.info/Elements/i/P40046) | **related item of item** || `Item` | U / S / Id / IRI | O | >1 |

[^1]: Vastlegging / *Recording method*, volgens <br>**U**: "unstructured"<br>**S**: "structured"<br>**Id**: "identifier" <br>**IRI**: IRI.
[^2]: Verplicht veld?, volgens <br>**M**: "*Must* / Verplicht"<br>**MA**: "*Must if applicable* / Verplicht indien van toepassing"<br>**O**: "*Optional* / Optioneel" 
