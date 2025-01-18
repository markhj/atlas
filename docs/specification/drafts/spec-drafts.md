@page spec-drafts Drafts of specifications

This page contains the "work in progress" of different unimplemented
schemas which may or may not become relevant in the future.

## Full basic country model

````json
{
    "codes": {
        "iso_3166_1": {
            "alpha_2": "DK",
            "alpha_3": "DNK",
            "numeric": 208
        }
    },
    "name": {
        "common_names": [
            "Denmark"
        ],
        "official_names": [
            "Kingdom of Denmark"
        ] 
    },
    "population": {
        "size": 5982117 
    },
    "demonyms": [
        "Danish",
        "Dane"
    ],
    "capital": {
        "capital": "Copenhagen",
        "de_jure": true
    },
    "languages": [
        {
            "iso_639_1": "da",
            "status": "official"
        },
        {
            "iso_639_1": "de",
            "status": "regional"
        }
    ],
    "tlds": [
        "dk"
    ],
    "calling_code": 45
}
````

## Note on names

Translations/localization is planned, but will not be added in this
file. Instead, translations will be provided in separate files which
have this exact purpose.

## Note on ``languages``

The locale code can be deduced from the ISO-639-1 code, combined
with the already provided ISO-3166 Alpha-2 code.

## Note on ``capital``

e.g. the situation in Switzerland:

````json
{
    "capital": "Bern",
    "de_jure": false
}
````
