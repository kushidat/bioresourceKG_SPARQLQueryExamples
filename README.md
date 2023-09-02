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
  - No. of federated queries: 0

The average runtime (10 times):  
- 1 seconds [Execution date: 1 September 2023]  
  
Results:
- No. of bioresources: 913
- No. of related genes: 76



## SPARQL Query Example 2 
[SPARQL_Query_Example2.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example2.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using federated search for Uniprot official SPARQL endpoint. 

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - _**SERVICE < uniprot >**_
    - GRAPH < rhea >
    - GRAPH < chebi >
  - Sub queries
    - nothing
  - No. of federated queries: 1 (UniProt)

The average runtime (10 times):  
- Virtuoso S1T00 Error SR171: Transaction timed out (over 10 minutes)
  
Results:
- No. of bioresources: ND
- No. of related genes: ND


## SPARQL Query Example 3 
[SPARQL_Query_Example3.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example3.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using federated search for Rhea official SPARQL endpoint. 

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - _**SERVICE < rhea >**_
    - GRAPH < chebi >
  - Sub queries
    - nothing
  - No. of federated queries: 1 (Rhea)

The average runtime (10 times):  
- Virtuoso S1T00 Error SR171: Transaction timed out (over 10 minutes)
  
Results:
- No. of bioresources: ND
- No. of related genes: ND


## SPARQL Query Example 4 
[SPARQL_Query_Example4.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example4.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using federated search for ChEBI’s SPARQL endpoint within RDF Portal. 

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < rhea >
    - _**SERVICE < chebi >**_
  - Sub queries
    - nothing
  - No. of federated queries: 1 (ChEBI)

The average runtime (10 times):  
- 502 Proxy Error
  
Results:
- No. of bioresources: ND
- No. of related genes: ND


## SPARQL Query Example 5  
[SPARQL_Query_Example5.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example5.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using subqueries but not using federated queries

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
  - Sub queries
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < rhea >
    - GRAPH < chebi >
  - No. of federated queries: 0

The average runtime (10 times):  
- 1 seconds [Execution date: 1 September 2023] 
  
Results:
- No. of bioresources: 913
- No. of related genes: 76


## SPARQL Query Example 6  
[SPARQL_Query_Example6.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example6.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using subqueries and federated queries for Uniprot official SPARQL endpoint. 

Search parameters:  
  - Main queries
    - _**SERVICE < uniprot >**_
  - Sub queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < rhea >
    - GRAPH < chebi >
  - No. of federated queries: 1 (UniProt)

The average runtime (10 times):  
-  seconds [Execution date: 1 September 2023] 
  
Results:
- No. of bioresources: 913
- No. of related genes: 76


## SPARQL Query Example 7  
[SPARQL_Query_Example7.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example7.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using subqueries and federated queries for Rhea official SPARQL endpoint. 

Search parameters:  
  - Main queries
    - _**SERVICE < rhea >**_
  - Sub queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < chebi >
  - No. of federated queries: 1 (Rhea)

The average runtime (10 times):  
-  seconds [Execution date: 1 September 2023] 
  
Results:
- No. of bioresources: 913
- No. of related genes: 76


## SPARQL Query Example 8  
[SPARQL_Query_Example8.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Example8.txt)  
Description: A SPARQL query for obtaining bioresources relevant to ChEBI role ([chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079)) using subqueries and federated queries for ChEBI’s SPARQL endpoint within RDF Portal. 

Search parameters:  
  - Main queries
    - _**SERVICE < chebi >**_
  - Sub queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < rhea >
  - No. of federated queries: 1 (ChEBI)

The average runtime (10 times):  
-  seconds [Execution date: 1 September 2023] 
  
Results:
- No. of bioresources: 913
- No. of related genes: 76
  
