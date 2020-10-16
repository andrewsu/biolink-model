---
parent: Classes
title: biolink:GenotypeAsAModelOfDiseaseAssociation
grand_parent: Browse Biolink Model
layout: default
---

# Class: GenotypeAsAModelOfDiseaseAssociation




URI: [biolink:GenotypeAsAModelOfDiseaseAssociation](https://w3id.org/biolink/vocab/GenotypeAsAModelOfDiseaseAssociation)


---

![img](http://yuml.me/diagram/nofunky;dir:TB/class/[SeverityValue],[Publication],[Provider],[OntologyClass],[Onset],[NamedThing],[ModelToDiseaseMixin],[GenotypeToDiseaseAssociation],[Genotype]%3Csubject%201..1-%20[GenotypeAsAModelOfDiseaseAssociation%7Crelation(i):uriorcurie;id(i):string;negated(i):boolean%20%3F],[GenotypeAsAModelOfDiseaseAssociation]uses%20-.-%3E[ModelToDiseaseMixin],[GenotypeAsAModelOfDiseaseAssociation]uses%20-.-%3E[EntityToDiseaseAssociation],[GenotypeToDiseaseAssociation]%5E-[GenotypeAsAModelOfDiseaseAssociation],[Genotype],[FrequencyValue],[EntityToDiseaseAssociation])

---


## Parents

 *  is_a: [GenotypeToDiseaseAssociation](GenotypeToDiseaseAssociation.md)

## Uses Mixins

 *  mixin: [ModelToDiseaseMixin](ModelToDiseaseMixin.md) - This mixin is used for any association class for which the subject (source node) plays the role of a 'model', in that it recapitulates some features of the disease in a way that is useful for studying the disease outside a patient carrying the disease
 *  mixin: [EntityToDiseaseAssociation](EntityToDiseaseAssociation.md) - mixin class for any association whose object (target node) is a disease

## Referenced by class


## Attributes


### Own

 * [genotype as a model of disease association➞subject](genotype_as_a_model_of_disease_association_subject.md)  <sub>REQ</sub>
    * Description: A genotype that has a role in modeling the disease.
    * range: [Genotype](Genotype.md)

### Inherited from association:

 * [subject](subject.md)  <sub>REQ</sub>
    * Description: connects an association to the subject of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [relation](relation.md)  <sub>REQ</sub>
    * Description: The relation which describes an association between a subject and an object in a more granular manner. Usually this is a term from Relation Ontology, but it can be any edge CURIE.
    * range: [Uriorcurie](types/Uriorcurie.md)
 * [object](object.md)  <sub>REQ</sub>
    * Description: connects an association to the object of the association. For example, in a gene-to-phenotype association, the gene is subject and phenotype is object.
    * range: [NamedThing](NamedThing.md)
 * [association➞id](association_id.md)  <sub>REQ</sub>
    * Description: A unique identifier for an association
    * range: [String](types/String.md)
    * in subsets: (translator_minimal)
 * [negated](negated.md)  <sub>OPT</sub>
    * Description: if set to true, then the association is negated i.e. is not true
    * range: [Boolean](types/Boolean.md)
 * [association type](association_type.md)  <sub>OPT</sub>
    * Description: connects an association to the type of association (e.g. gene to phenotype)
    * range: [OntologyClass](OntologyClass.md)
 * [qualifiers](qualifiers.md)  <sub>0..*</sub>
    * Description: connects an association to qualifiers that modify or qualify the meaning of that association
    * range: [OntologyClass](OntologyClass.md)
 * [publications](publications.md)  <sub>0..*</sub>
    * Description: connects an association to publications supporting the association
    * range: [Publication](Publication.md)
 * [provided by](provided_by.md)  <sub>0..*</sub>
    * Description: connects an association to the agent (person, organization or group) that provided it
    * range: [Provider](Provider.md)

### Inherited from entity to feature or disease qualifiers:

 * [severity qualifier](severity_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state how severe the phenotype is in the subject
    * range: [SeverityValue](SeverityValue.md)
 * [onset qualifier](onset_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state when the phenotype appears is in the subject
    * range: [Onset](Onset.md)

### Inherited from frequency qualifier mixin:

 * [frequency qualifier](frequency_qualifier.md)  <sub>OPT</sub>
    * Description: a qualifier used in a phenotypic association to state how frequent the phenotype is observed in the subject
    * range: [FrequencyValue](FrequencyValue.md)

### Inherited from genotype to disease association:

 * [genotype to disease association➞subject](genotype_to_disease_association_subject.md)  <sub>REQ</sub>
    * Description: a genotype that is associated in some way with a disease state
    * range: [NamedThing](NamedThing.md)
 * [genotype to disease association➞relation](genotype_to_disease_association_relation.md)  <sub>REQ</sub>
    * Description: E.g. is pathogenic for
    * range: [Uriorcurie](types/Uriorcurie.md)
 * [genotype to disease association➞object](genotype_to_disease_association_object.md)  <sub>REQ</sub>
    * Description: a disease that is associated with that genotype
    * range: [NamedThing](NamedThing.md)
    * Example:    

### Domain for slot:

 * [genotype as a model of disease association➞subject](genotype_as_a_model_of_disease_association_subject.md)  <sub>REQ</sub>
    * Description: A genotype that has a role in modeling the disease.
    * range: [Genotype](Genotype.md)