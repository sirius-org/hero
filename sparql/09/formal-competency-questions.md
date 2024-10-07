# Formal Competency Questions

## CQ_9.1
Which objects are used by analysis activities as bases for their statements referring to the probable estimate of magnitude of risk?

```SPARQL
PREFIX : <https://w3id.org/sirius/ontology/data/09/>
PREFIX aat: <http://vocab.getty.edu/page/aat/>
PREFIX hero: <https://w3id.org/sirius/ontology/hero/>
PREFIX wd: <http://www.wikidata.org/entity/>

SELECT ?activity ?probable_estimate_value ?object
WHERE {
  ?activity a hero:Activity ;
    hero:hasType wd:Q217602 ;
    hero:uses ?object ;
    hero:assigns ?statement .
  ?statement hero:hasType aat:300435430 ;
    hero:refersTo ?concept .
  ?concept hero:hasType ?type ;
    hero:hasComponent ?prob_estimate .
  ?prob_estimate hero:hasType wd:Q226995 ;
    hero:hasValue ?probable_estimate_value .
}
```

## CQ_9.2
What are the objects motivating the evaluation activities?

```SPARQL
PREFIX : <https://w3id.org/sirius/ontology/data/09/>
PREFIX aat: <http://vocab.getty.edu/page/aat/>
PREFIX hero: <https://w3id.org/sirius/ontology/hero/>
PREFIX wd: <http://www.wikidata.org/entity/>

SELECT ?activity ?object
WHERE {
  ?activity a hero:Activity ;
    hero:hasType wd:Q1379672 ;
    hero:isMotivatedBy ?object ;
    hero:assigns ?statement .
}
```
