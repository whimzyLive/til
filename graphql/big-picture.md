# GraphQL: The Big Picture

## What is GraphQL
- Move the focus of development to client apps
- Provides flexibility and efficiency between client and server applications
- GraphQL eliminates the under-fatching, over-fatching and unnecessary network round trips issue
- GraphQL doesn't use HTTP spec for caching and relys on development frameworks to do the heavy lifting

## GraphQL Core Concepts
- Bult in scalar types - `Int`, `Float`, `String`, `Boolean`, `Id`, `Enums`
- Each schema contains at minimum `Query` and/or `Mutation` type
- Queries - Used to query data - queries on all fields run in parallel 
- Queries Fields - Only returns fields requested by client
- Queries Arguments - Used to pass arguments to fields, each field and nested object can get its own set of arguments
- Queries Aliases - Used to renmae the result of a field with a given alias
- Queries Fragments - Reusable units in GraphQL - like functions in any other language
- Queries Variables - Used to make qraphql query dynamic
- Mutation - Used to create/update/delete data - mutation always run in sequence
