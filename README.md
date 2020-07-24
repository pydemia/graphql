# graphql

## Features

### Types
The GraphQL type system supports the following kind of types:

* Scalar
* Object
* Interface
* Union
* InputObject
* Enum


### Schema

* DataFetcher: 
  - query: Provides the data for a filed.
  - mutation: query + changes something, as POST(or PUT)
  
  Every `field` definition has a DataFetcher. when not configured, `PropertyDataFetcher` is used. It fetches data from Map & Java Beans.
  
* TypeResolver: helps `graphql-java` to decide which type a concrete value belongs to. It is needed for `Interface` and `Union`.

