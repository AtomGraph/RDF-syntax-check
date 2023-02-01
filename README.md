# RDF syntax check
GH action that iterates all RDF files in the repository and validates their syntax using [Apache Jena's riot parser](https://jena.apache.org/documentation/io/#command-line-tools).
The action fails as soon as an invalid file is detected.