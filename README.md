# Translate
## Description
Translate text with deepl

## Dotenv
Create a .env file
```
DEEPL_KEY=api key
```

## Usage
```
Usage : translate <option> [text]

Option :
-h or --help ........................... Show help
-v or --version ........................ Show version
-s <lang> .............................. Source language
-t <lang> .............................. Target language

Example :
translate -t fr "Hello World!"
echo "Hello World!" | translate -t fr
```
