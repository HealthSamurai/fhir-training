# FHIR 

## Overview

* Is Interoperability your problem?
  * Language

* Invent your standard (exercise)
* History of Health IT Standards
  * HL7v2.x
  * HL7v3 & RIM
  * CDA
  * OpenEHR
  * IHE Profiles
  * FHIR

* Why FHIR?
  * ...

* FHIR overview 
  * Resources (Informational Model)
    * Extensions
    * Profiles
    * Mapping & Fitting
    * Formats (JSON, XML, Tortoise)
  * REST API and other paradigms (Operational Model)
    * CRUD (Patch?)
    * Search
      * Search Parameters
      * Chained Search
      * include
    * History
    * Transaction
    * Messaging paradigm
    * Document paradigm
  * Terminology (Semantic Model)
    * CodeSystem
      * ICD-10
      * SnomedCT
      * Loinc
      * RxNorm (US)
    * ValueSet 
    * ConceptMap
    * Terminology API 
      * ...
  * Tools
    * servers
    * libraries

* How to use FHIR

  *  Protocol?
  *  Infromation Model
  *  Expert's community
  *  Tools

## FHIR Client

* FHIR Client
  * FHIR servers
  * FHIR Client libraries && tools (POSTman, curl)
  * List patients
  * Search patients
  * Create patient
  * Map your patient to FHIR patient
  * Extend patient
  * Create Encounter
  * Chained params and _include
  * Bundle
  * Transaction
  * Terminology
  
* Security and Access Control 
  * OAUTH intro
  * OAUTH client for FHIR server
  * Scopes 
  * Access Control
    * RBAC
    * ACL
    * Policies


## FHIR server

* Conformance Resource
* StructureDefinition, Search Paramenters
* fhirbase 
  * Implementing FHIR search
   * Search Paramenters
   * chained params
   * includes
* TestScript
* Implementing Terminology
* Real World Cases

## FHIR in real world

* Argonaut
* Community
* Smart on FHIR
* Road Map
* Projects 


## FHIR unsolved problems

* Multi-Versions
* Profiling & Extensions 
* Mapping to other standards
* Interoperable Security
* Bridge to other standards (Swagger, GraphQL etc)
* Subscribtions & Replication
