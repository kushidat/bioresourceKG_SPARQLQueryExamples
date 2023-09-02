# bioresourceKG_SPARQLQueryExamples
Lists of SPARQL query examples for [RIKEN Bioresouce KG](https://github.com/kushidat/bioresourceKG_schema).   
RIKEN BioResouce MetaDatabase SPARQL endpoint: https://knowledge.brc.riken.jp/sparql
___
## SPARQL Query Example 1  
[SPARQL_Query_Example1.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example1.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079))  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch > 
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < rhea >
    - GRAPH < chebi >
  - Sub queries
    - nothing

The average runtime (10 times):  
- 1 seconds [Execution date: 1 September 2023]  
  
Results:
- No. of bioresources: 913
- No. of related genes: 76
