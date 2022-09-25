# Translate
## Description
Translate text with deepl

## Dotenv
```
DEEPL_KEY=api key
```

## Usage
Usage : translate [option] <text>

Option :
-h or --help ........................... Show help
-v or --version ........................ Show version
-s <lang> .............................. Source language
-t <lang> .............................. Target language
- ...................................... Stdin

Example :
translate -t FR "Hello World!"
echo "Hello World!" | translate -t FR -
