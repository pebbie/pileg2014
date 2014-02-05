Tampilkan seluruh nama caleg yang merupakan guru besar (bergelar Prof.)
==   
 
    PREFIX pemilu: <http://pebbie.org/ont/2014/pemilu#>
    SELECT ?nama 
    WHERE {
        ?c a pemilu:Caleg .
        ?c rdfs:label ?nama .
        FILTER REGEX(?nama, "Prof", "i")
    }