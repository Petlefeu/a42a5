# A4 to A5

[![Build Status](https://travis-ci.org/nbeguier/a42a5.svg?branch=master)](https://travis-ci.org/nbeguier/a42a5) [![Python 3.4|3.7](https://img.shields.io/badge/python-3.4|3.7-green.svg)](https://www.python.org/) [![License](https://img.shields.io/badge/Licence-Apache%202.0-blue.svg)](https://github.com/nbeguier/a42a5/blob/master/LICENSE)

## Prerequisites

```bash
pip3 install -r requirements.txt
```

## Usage

```bash
# python3 a42a5.py --help
usage: a42a5.py [-h] [--up UP] [--down DOWN] [--left LEFT] [--right RIGHT]
                [--inter INTER] [--reverse]
                input output

positional arguments:
  input          Input file
  output         Output file

optional arguments:
  -h, --help     show this help message and exit
  --up UP        Margin up
  --down DOWN    Margin down
  --left LEFT    Margin left
  --right RIGHT  Margin right
  --inter INTER  Intersection between two pages
  --reverse      Cut vertically rather than horizontally
```

## Examples

```bash
# Easy use
python3 a42a5.py PDF_Samples/example_A4.pdf output_A5.pdf

# More complex
python3 a42a5.py PDF_Samples/example_A4.pdf output_A5.pdf --up 100 --down 100 --left 10 --right 5 --inter 20

# Cut horizontally
python3 a42a5.py PDF_Samples/example_A4.pdf output_A5.pdf --reverse
```
