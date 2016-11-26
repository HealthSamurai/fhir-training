# REST API


## Whole System Interactions

* conformance Get a conformance statement for the system
* batch/transaction Update, create or delete a set of resources in a single interaction
* history Retrieve the change history for all resources
* search Search across all resource types based on some filter criteria

## Instance Level Interactions

* read Read the current state of the resource
* vread Read the state of a specific version of the resource
* update Update an existing resource by its id (or create it if it is new)
* delete Delete a resource
* history Retrieve the change history for a particular resource

## Type Level Interactions

* create Create a new resource with a server assigned id
* search Search the resource type based on some filter criteria
* history Retrieve the change history for a particular resource type




## Basics

* Read: `GET [base]/[type]/[id]`
* Create: `POST [base]/[type]`
* Update: `POST [base]/[type]/[id]`
* Search: `GET [base]/[type]`
* History: `GET [base]/[type]/[id]/_history/[vid]`

