## Inheretance

Resource -> DomainResource -> Patient

## [Resource](http://hl7.org/fhir/2016Sep/resource.html#resource)

```yaml
Resource:
  id: {card: [0,1], type: "id"}
  meta: {card: [0,1], type: "Meta"}
  ...
```

## [Meta](http://hl7.org/fhir/2016Sep/resource.html#Meta)

```yaml
Meta:
  versionId: {type: "id"}
  lastUpdated: {type: "instant"}
  profile: {card: "*"}
```

## [DomainResource](http://hl7.org/fhir/2016Sep/domainresource.html#bnr)

```yaml
DomainResource:
  text: {type: "Narrative"}
  contained: {card: "*", type: "Resource"}
  profile: {card: "*"}
```

## [Patient](http://hl7.org/fhir/2016Sep/patient.html#resource)

```yaml
Patient:
  active: {type: boolean, card: 0..1}
  name: {type: HumanName, card: *}
  identifier: {type: Identifier, card: *}
  deceased[x]: 
    boolean: ...
    datetime: ...
  contact:
    relationship: {}
    telecom: {}
```

## [StructureDefinition](http://hl7.org/fhir/2016Sep/structuredefinition.html#resource)


```
StructureDefinition:
  kind: primitive-type | complex-type | resource | logical
  abstract: ???
  baseDefinition: parent
  derivation: specialization | constraint
  snapshot: ElementDefinition
  differential: ElementDefinition

ElementDefinition:
  path: 'Patient.name'
  min: 0,1,...
  max: 0,1,...,*
  type:
    code: 'HumanName'
    ...
  constraint: 0..*
    expression: string

  binding: 0..1
    strength: ENUM: required | extensible | preferred | example
    valueSetReference: ref

```

## Patient Example:

```yaml
Patient.snapshot:
  ...
  - id: "Patient.address"
    path: "Patient.address"
    short: "Addresses for the individual"
    min: 0
    max: "*"
    type: [{code: "Address"}]
    isSummary: true
    mapping: 
      - identity: "v2"
        map: "PID-11"
      - identity: "rim"
        map: "addr"
      - identity: "cda"
        map: ".addr"
  ...
```
