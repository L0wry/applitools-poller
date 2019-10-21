# Applitools Poller

## Concept

Applitools is a great tool but is hard to run in CI due to it's limited integrations.

This tools aims to make integration with Applitools easier by returning if a test run has passed or failed on a batch ID.
(For example it could be used as a branch policy on azure dev ops 🤮 (If only I could use Github).)

This tool has been built to run on an Azure functions.

Make a get request to the deployed function with the following.

`?batchKey=applitoolsBatchID`

`?ApiKey=applitoolsApiKey`

## Example
`axios.get(`${BASE_URL}?apiKey=${apiKey}&batchId=${batchId}`)`

## Installing dependancies
`yarn`

## Running Tests
`yarn test`

##
