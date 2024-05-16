# Formal Competency Questions
## CQ_4.1
Which assets are part of the house asset, and what is the percentage each asset represents, ordered in descending order?

```SPARQL
PREFIX tbox: <https://w3id.org/sirius/ontology/development/04/schema/>
PREFIX abox: <https://w3id.org/sirius/ontology/development/04/data/>

SELECT DISTINCT ?asset ?asset_part ?percentage
WHERE {
  ?asset a tbox:HeritageAsset ;
        tbox:hasPart ?asset_part .
  ?value_assessment tbox:describes ?asset_part ;
                        tbox:assessesPercentage ?percentage .
}
```

***

## CQ_4.2
What are the contributing values assigned to an asset, and what is their associated score, dimension, aspect, note, documentation, and time interval?

```SPARQL
PREFIX tbox: <https://w3id.org/sirius/ontology/development/04/schema/>
PREFIX abox: <https://w3id.org/sirius/ontology/development/04/data/>

SELECT DISTINCT ?asset_part ?value ?score ?dimension ?aspect ?note ?document ?time_interval_start ?time_interval_end
WHERE {
    ?asset a tbox:HeritageAsset ;
            tbox:hasPart ?asset_part .
    ?value_assessment tbox:describes ?asset_part ;
                        tbox:assigns ?value ;
                        tbox:withinDimension ?dimension ;
                        tbox:withinAspect ?aspect ;
                        tbox:hasNote ?note ;
                        tbox:isDocumentedBy ?document ;
                        tbox:atTime ?time_interval .
    ?value tbox:hasScore ?score .
    ?time_interval tbox:hasStartDate ?time_interval_start ;
                    tbox:hasEndDate ?time_interval_end .
}
```
