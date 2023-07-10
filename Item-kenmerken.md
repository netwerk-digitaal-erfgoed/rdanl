Toe te passen RDA-kenmerken voor Item-entiteiten {#item-kenmerken}
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
            <td>[rdai:P40001](http://rdaregistry.info/Elements/i/P40001)</td>
            <td>**identifierForItem**</td>
            <td></td>
            <td>`Nomen`</td>
            <td>Id</td>
            <td>M</td>
            <td>1</td>
            <td>barcode, URN</td>
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
            <td>[rdai:P40049](http://rdaregistry.info/Elements/i/P40049)</td>
            <td>**manifestationExemplified**</td>
            <td></td>
            <td>`Manifestation`</td>
            <td>S / Id / IRI</td>
            <td>M</td>
            <td>1</td>
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
            <td>[rdai:P40028](http://rdaregistry.info/Elements/i/P40028)</td>
            <td>**noteOnItem**</td>
            <td>voor het signatuur heeft RDA geen element, daarom kan indien gewenst het signatuur in edit met voorlooptekst &quot;Signatuur:&quot; opgenomen worden</td>
            <td></td>
            <td>U</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdai:P40048](http://rdaregistry.info/Elements/i/P40048)</td>
            <td>**restrictionOnUseOfItem**</td>
            <td></td>
            <td></td>
            <td>U / S / Id / IRI</td>
            <td>MA</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdai:P40096](http://rdaregistry.info/Elements/i/P40096)</td>
            <td>**categoryOfItem**</td>
            <td></td>
            <td></td>
            <td>U / S / Id / IRI</td>
            <td>O</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td></td>
            <td>*General relationships:*</td>
            <td>*algemene elementen om relaties van de entiteit te beschrijven (basistoepassingsprofiel):*</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>[rdai:P40162](http://rdaregistry.info/Elements/i/P40162)</td>
            <td>**locationOfItem**</td>
            <td></td>
            <td>`Place`</td>
            <td>S</td>
            <td>M</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdai:P40136](http://rdaregistry.info/Elements/i/P40136)</td>
            <td>**ownerCorporateBody**</td>
            <td></td>
            <td>`CorporateBody`</td>
            <td>S / Id / IRI</td>
            <td>M</td>
            <td>1</td>
            <td></td>
        </tr>
        <tr>
            <td>[rdai:P40046](http://rdaregistry.info/Elements/i/P40046)</td>
            <td>**related item of item**</td>
            <td></td>
            <td>`Item`</td>
            <td>U / S / Id / IRI</td>
            <td>O</td>
            <td>&gt;1</td>
            <td></td>
        </tr>
    </tbody>
</table>
