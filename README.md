# Translate

## Description

Translate text with deepl

## Required Dependencies

-   `jq`

## Available engine

-   [deepl](https://www.deepl.com)
-   [libre](https://github.com/LibreTranslate/LibreTranslate)

## Installation

1. Clone the repository:

```bash
git clone https://github.com/LordPax/translate.git
cd translate
```

2. Execute the script to generate config file in `.config/translate`

```bash
./translate
```

3. Create dotenv file `~/.config/translate/.env` with

```bash
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
