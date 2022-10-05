# Translate
## Description
Translate text with deepl

## Evailable engine
* [deepl](https://www.deepl.com)
* [libre](https://github.com/LibreTranslate/LibreTranslate)

## Dotenv
Create a .env file
```
DEEPL_ROUTE=https://api-free.deepl.com/v2/translate
DEEPL_KEY=mandatory if you use deepl
LIBRE_ROUTE_DETECT=localhost:5000/detect
LIBRE_ROUTE=localhost:5000/translate
LIBRE_KEY=not mandatory if route is on localhost
```

## Usage
```
Usage : translate <option> [text]

Option :
-h or --help ........................... Show help
-v or --version ........................ Show version
-e or --engine <engine> ................ Set engine (default : deepl)
-s <lang> .............................. Source language
-t <lang> .............................. Target language

Engine :
* deepl
* libre

Example :
translate -t fr "Hello World!"
echo "Hello World!" | translate -t fr
```
