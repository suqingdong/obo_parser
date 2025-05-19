# A Python library for parsing OBO (Open Biological and Biomedical Ontologies) files.

This is a Python library for parsing OBO files. It is based on the [OBO format specification](http://owl.cs.manchester.ac.uk/oboformat/doc/obo-syntax.html) and is designed to be easy to use and flexible.

## Installation

```
pip install obo_parser
```

## Usage

### Use in Commmand Line

```bash
obo_parser headers -f path/to/obo_file.obo
obo_parser headers -f path/to/obo_file.obo -o headers.json

obo_parser terms -f path/to/obo_file.obo
obo_parser terms -f path/to/obo_file.obo -o terms.jl
```

### Use in Python

```python
from obo_parser.parser import OBO_Parser

obo = OBO_Parser('./hp.obo')
print(obo.headers)

for term in obo.terms:
    print(term)

```


