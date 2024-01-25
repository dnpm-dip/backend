# DNPM:DIP - Backend

Umbrella project for the modules/projects composing the DNPM:DIP backend.

## Base Components

* [Core](https://github.com/KohlbacherLab/dnpm-dip-core): Utilities, Base components for Coding management, Base domain modelling components

* [Service Base](https://github.com/KohlbacherLab/dnpm-dip-service-base): Base components for use-case specific service implementations

* [Connector Base](https://github.com/KohlbacherLab/dnpm-dip-connector-base): Base implementations of abstract Connector defined in [service base](https://github.com/KohlbacherLab/dnpm-dip-service-base)


## Catalog / CodeSystem Components

* [ICD Catalogs](https://github.com/KohlbacherLab/dnpm-dip-icd-catalogs): ICD-10-GM and ICD-O-3 CodeSystem provider implementations

* [ATC Medication Catalog](https://github.com/KohlbacherLab/dnpm-dip-atc-catalog): CodeSystem provider implementation for ATC medication catalog

* [HGNC Gene Set](https://github.com/KohlbacherLab/dnpm-dip-hgnc-catalog): CodeSystem provider implementation for [HGNC Gene Set](https://www.genenames.org/download/statistics-and-files/)

* [Catalog Service](https://github.com/KohlbacherLab/dnpm-dip-catalog-service): Component to load all CodeSystemProvider plugins according to the Service Provider Interface (SPI) Pattern (see [CodeSystemProvider](https://github.com/KohlbacherLab/dnpm-dip-core/blob/main/src/main/scala/de/dnpm/dip/coding/CodeSystemProvider.scala)) 


## Use Case Modules

### Rare Diseases (RD)

* [RD Model](https://github.com/KohlbacherLab/dnpm-dip-rd-model): RD Domain/Data Model and object generators, together with CodeSystem provider implementations for [Human Phenotype Ontology](https://hpo.jax.org/app/) (HPO) and [Orphanet Rare Disease Ontology](https://www.orphadata.com/ordo/) (ORDO)

* [RD Query Service](https://github.com/KohlbacherLab/dnpm-dip-rd-query-service): RD-specific implementation of Query Service from [service base](https://github.com/KohlbacherLab/dnpm-dip-service-base)


### Molecular Tumor Board (MTB)

* [MTB Model](https://github.com/KohlbacherLab/dnpm-dip-mtb-model): MTB Domain/Data Model and object generators

* [MTB Query Service](https://github.com/KohlbacherLab/dnpm-dip-mtb-query-service): MTB-specific implementation of Query Service from [service base](https://github.com/KohlbacherLab/dnpm-dip-service-base)



## Backend Deployable

[REST API Gateway](https://github.com/KohlbacherLab/dnpm-dip-api-gateway): The above use case modules/services are bundled and exposed RESTfully via an API Gateway


## Other Dependencies

* [Data Object Generator Library](https://github.com/KohlbacherLab/Generators)

