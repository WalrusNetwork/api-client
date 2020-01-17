# Java GraphQL Client for Walrus API
This utilises the Apollo Android GraphQL library to automatically generate GraphQL files.

## Building
Just run `./gradlew jar` and pull the jar out of `build/`.

## Updating
1. Download a new schema.json. You can do that using the apollo cli by following the instructions [here](https://github.com/apollographql/apollo-android#downloading-a-schemajson-file).
2. Update the graphql files with the new queries you'd like classes generated for. Please not that these graphql files are not the same as what is used on the server and have odd syntax. Client-side graphql files are different from what's used server-side. You can see some example syntax [here](https://github.com/apollographql/apollo-android/tree/master/samples/java-sample/src/main/graphql/com/apollographql/apollo/sample).
3. Run `./gradlew generateApolloClasses`.
4. Feel free to build the jar when ready, deploy to CI, and update the dependent projects.
