# RDF syntax check
GH action that iterates all RDF files in the repository and validates their syntax using [Apache Jena's riot parser](https://jena.apache.org/documentation/io/#command-line-tools).
The action fails as soon as an invalid file is detected.

## Usage example

```yml
name: RDF data validation

on: push

jobs:
  rdf-syntax-check:
    runs-on: ubuntu-latest
    steps:
      - name: RDF syntax check
        uses: AtomGraph/RDF-syntax-check@v1.0.4
```