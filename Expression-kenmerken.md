Toe te passen RDA-kenmerken voor Expression-entiteiten {#expression-kenmerken}
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
            <th></th>
            <th></th>
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
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20312](http://rdaregistry.info/Elements/e/P20312)</td>
            <td>**titleOfExpression**</td>
            <td></td>
            <td>`Nomen`</td>
            <td>U</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20002](http://rdaregistry.info/Elements/e/P20002)</td>
            <td>**identifierForExpression**</td>
            <td>niet bedoeld voor de IRI van de entiteit zelf</td>
            <td>`Nomen`</td>
            <td>identifier/iri</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan=2>*Coherence*:</td>
            <td>*primaire relaties tussen entiteiten:*</td>
            <td></td>
            <td></td>
            <td>M</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20231](http://rdaregistry.info/Elements/e/P20231)</td>
            <td>**workExpressed**</td>
            <td></td>
            <td>`Work`</td>
            <td>S / Id / IRI</td>
            <td>M</td>
            <td>1</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20059](http://rdaregistry.info/Elements/2/P20059)</td>
            <td>**manifestationOfExpression**</td>
            <td>relateer `Manifestations` aan de `Expression` vooral via de `Manifestation`</td>
            <td>`Manifestation`</td>
            <td>S / Id / IRI</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
            <td></td>
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
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20001](http://rdaregistry.info/Elements/e/P20001)</td>
            <td>**contentType**</td>
            <td></td>
            <td>-</td>
            <td>S / IRI</td>
            <td>M</td>
            <td>&gt;1</td>
            <td>[RDA Content Type](http://www.rdaregistry.info/termList/RDAContentType/?language=nl)</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20006](http://rdaregistry.info/Elements/e/P20006)</td>
            <td>**languageOfExpression**</td>
            <td></td>
            <td></td>
            <td>S</td>
            <td>M</td>
            <td>&gt;1</td>
            <td>ISO 639.2</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20071](http://rdaregistry.info/Elements/e/P20071)</td>
            <td>**noteOnExpression**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20069](http://rdaregistry.info/Elements/e/P20069)</td>
            <td>**summarizationOfContent**</td>
            <td></td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td colspan=2>*General relationships:*</td>
            <td>*algemene elementen om relaties van de entiteit te beschrijven (basistoepassingsprofiel):*</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20214](http://rdaregistry.info/Elements/e/P20214)</td>
            <td>**dateOfExpression**</td>
            <td></td>
            <td>`Timespan`</td>
            <td>U / S / Id / IRI</td>
            <td>MA</td>
            <td>1</td>
            <td>ISO 8601-1:2019</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20053](http://rdaregistry.info/Elements/e/P20053)</td>
            <td>**creatorAgentOfExpression**</td>
            <td>gebruik een zo specifiek mogelijke narrow element</td>
            <td>`Agent`</td>
            <td>S / Id / IRI</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td>NTA, NACO, Corporatiethesaurus</td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20325](http://rdaregistry.info/Elements/e/P20325)</td>
            <td>**representativeExpressionOf**</td>
            <td>gebruik dit element in ieder geval voor de Expression van de eerste Manifestation van het Work als meerdere Expressions aanwezig zijn</td>
            <td>`Work`</td>
            <td>S / Id / IRI</td>
            <td>O</td>
            <td>1</td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20205](http://rdaregistry.info/Elements/e/P20205)</td>
            <td>**relatedExpressionOfExpression**</td>
            <td>gebruik een zo specifiek mogelijk subelement, oa. voor vertalingen en bewerkingen</td>
            <td>`Expression`</td>
            <td>S / Id / IRI</td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
            <td></td>
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
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdae:P20322](http://rdaregistry.info/Elements/e/P20322)</td>
            <td>**intendedAudienceOfExpression**</td>
            <td></td>
            <td></td>
            <td>U / S / Id / IRI</td>
            <td></td>
            <td>MA</td>
            <td>&gt;1</td>
            <td></td>
            <td>gebruik zoveel mogelijk een gecontroleerde waardelijst</td>
        </tr>
        <tr>
            <td>[rdae:P20219](http://rdaregistry.info/Elements/e/P20219)</td>
            <td>**duration**</td>
            <td>voor gebruik bij luisterboeken</td>
            <td></td>
            <td>S</td>
            <td></td>
            <td>MA</td>
            <td>1</td>
            <td>ISO 8601-1:2019</td>
            <td></td>
        </tr>
    </tbody>
</table>
