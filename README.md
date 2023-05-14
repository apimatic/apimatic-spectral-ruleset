# APIMatic Spectral Custom Ruleset

Generating code libraries for SDKs from API definitions require specific validation rules to ensure high quality code and accompanying documentation. 

We've developed this custom Spectral ruleset for those generating code from their OpenAPI definition with APIMatic.

## How to use the APIMatic rulset

Install Spectral following [these instructions](https://github.com/stoplightio/spectral#-installation).

Clone this repository and copy your API definition into the repository at the same level the .apimatic.yaml file.

Replace petstore-good.yaml with your API definition file name and run the command.

```
spectral lint petstore-good.yaml --ruleset .apimatic.yaml
```

## Current Ruleset

Below are the rules defined in .apimatic.yaml

* Property must include description
* Property must include an example
* Parameters must include description
* Parameters must include examples
* Request body must include description
* Request body must include examples
* Schemas must include description
* Schemas must include examples
* Response content must include examples

## Roadmap

Add more rules to improve the quality of generated SDKs