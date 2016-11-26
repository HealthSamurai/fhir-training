## Conformance

> A conformance statement is a set of capabilities of a FHIR Server that may be
> used as a statement of actual server functionality or a statement of required
> or desired server implementation.


```yaml

Conformance:
  rest: 0..*
    interaction: *
      code: transaction | batch | search-system | history-system
    searchParam:
      -- global search parameters
    resource: *
      type: Patient
      versioning: no-version | versioned | versioned-update
      readHistory: true
      updateCreate: true
      conditionalUpdate: true
      conditionalCreate: true
      searchParam:
        name: ...
        definition: ...
        type: number | date | string | token | reference | composite | quantity | uri
    operation: *
      -- link to OperationDefinition
    compartment: *
      -- link to CompartmentDefinition

```
