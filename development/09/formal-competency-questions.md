# Formal Competency Questions

## CQ_9.1
Which objects are used by analysis activities as bases for their statements referring to the probable estimate of magnitude of risk?

```SPARQL
PREFIX tbox: <https://w3id.org/sirius/ontology/development/09/schema/>
PREFIX : <https://w3id.org/sirius/ontology/development/09/data/>

SELECT ?activity ?probable_estimate_value ?object
WHERE {
  ?activity a tbox:AssessmentActivity ;
    tbox:hasType tbox:risk-analysis ;
    tbox:uses ?object ;
    tbox:assigns ?statement .
  ?statement tbox:hasType tbox:dimensions-description ;
    tbox:refersTo ?concept .
  ?concept tbox:hasType ?type ;
    tbox:isComposedOf ?prob_estimate .
  ?prob_estimate tbox:hasType tbox:probable-estimate ;
    tbox:hasValue ?probable_estimate_value .
}
```

## CQ_9.2
What are the objects motivating the evaluation activities?

```SPARQL
PREFIX tbox: <https://w3id.org/sirius/ontology/development/09/schema/>
PREFIX : <https://w3id.org/sirius/ontology/development/09/data/>

SELECT ?activity ?object
WHERE {
  ?activity a tbox:AssessmentActivity ;
    tbox:hasType tbox:risk-evaluation ;
    tbox:isMotivatedBy ?object ;
    tbox:assigns ?statement .
}
```
