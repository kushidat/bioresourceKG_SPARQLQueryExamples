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
    - Nothing
  - No. of federated queries: 0

The average runtime (10 times):  
- 1 seconds [Execution date: 1 September 2023]  
  
Results:
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): 913
- No. of the related genes: 76


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
    - Nothing
  - No. of federated queries: 1 (UniProt)

The average runtime (10 times):  
- Virtuoso S1T00 Error SR171: Transaction timed out (over 10 minutes)
  
Results:
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): ND
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
    - Nothing
  - No. of federated queries: 1 (Rhea)

The average runtime (10 times):  
- Virtuoso S1T00 Error SR171: Transaction timed out (over 10 minutes)
  
Results:
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): ND
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
    - Nothing
  - No. of federated queries: 1 (ChEBI)

The average runtime (10 times):  
- 502 Proxy Error
  
Results:
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): ND
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
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): 913
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
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): 913
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
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): 913
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
- No. of bioresources relevant to [chebi:67079](http://purl.obolibrary.org/obo/CHEBI_67079): 913
- No. of related genes: 76
  

## SPARQL Query Statistics 1  
[SPARQL_Query_Statistics1_plantD_role.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics1_plantD_role.txt)  
Description: A SPARQL query for obtaining plant DNA materials relevant to ChEBI roles. 

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < rhea >
    - GRAPH < chebi >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of ChEBI roles | No. of plant DNA materials<br> relevant to ChEBI roles (A) | No. of total<br> plant DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 164 | 62,244 | 291,583 | 0.21 |   

  
## SPARQL Query Statistics 2  
[SPARQL_Query_Statistics2_plantD_BA.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics2_plantD_BA.txt)  
Description: A SPARQL query for obtaining plant DNA materials relevant to KNApSAcK biological activities.

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_enzyme >
    - GRAPH < rhea >
    - GRAPH < knapsackCore >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of KNApSAcK<br> biological activities | No. of plant DNA materials<br> relevant to biological activities (A) | No. of total<br> plant DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 270 | 5,488 | 291,583 | 0.02 |   


## SPARQL Query Statistics 3  
[SPARQL_Query_Statistics3_plantD_MF.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics3_plantD_MF.txt)  
Description: A SPARQL query for obtaining plant DNA materials relevant to GO molecular functions.  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_go >
    - GRAPH < GO >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of GO<br> molecular functions | No. of plant DNA materials<br> relevant to molecular functions (A) | No. of total<br> plant DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 2,819 | 221,832 | 291,583 | 0.76 |   


## SPARQL Query Statistics 4  
[SPARQL_Query_Statistics4_plantD_BP.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics4_plantD_BP.txt)  
Description: A SPARQL query for obtaining plant DNA materials relevant to GO biological processes.  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_go >
    - GRAPH < GO >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of GO<br> biological processes | No. of plant DNA materials<br> relevant to biological processes (A) | No. of total<br> plant DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 3,949 | 224,752 | 291,583 | 0.77 |   


## SPARQL Query Statistics 5  
[SPARQL_Query_Statistics5_plantD_CC.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics5_plantD_CC.txt)  
Description: A SPARQL query for obtaining plant DNA materials relevant to GO cellular components.  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_go >
    - GRAPH < GO >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of GO<br> cellular components | No. of plant DNA materials<br> relevant to cellular components (A) | No. of total<br> plant DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 827 | 236,337 | 291,583 | 0.81 |   


## SPARQL Query Statistics 6  
[SPARQL_Query_Statistics6_humanD_MF.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics6_humanD_MF.txt)  
Description: A SPARQL query for obtaining human DNA materials relevant to GO molecular functions.  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_go >
    - GRAPH < GO >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of GO<br> molecular functions | No. of human DNA materials<br> relevant to molecular functions (A) | No. of total<br> human DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 4,441 | 94,960 | 125,856 | 0.75 |   


## SPARQL Query Statistics 7  
[SPARQL_Query_Statistics7_humanD_BP.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics7_humanD_BP.txt)  
Description: A SPARQL query for obtaining human DNA materials relevant to GO biological processes.  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_go >
    - GRAPH < GO >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of GO<br> biological processes | No. of human DNA materials<br> relevant to biological processes (A) | No. of total<br> human DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 12,606 | 101,715 | 125,856 | 0.81 |   


## SPARQL Query Statistics 8  
[SPARQL_Query_Statistics8_humanD_CC.txt](https://github.com/kushidat/bioresourceKG_SPARQLQueryExamples/blob/main/SPARQL_Query_Statistics8_humanD_CC.txt)  
Description: A SPARQL query for obtaining plant DNA materials relevant to GO cellular components.  

Search parameters:  
  - Main queries
    - GRAPH < xsearch_plant_xsearch >
    - GRAPH < uniprot_ncbigene >
    - GRAPH < uniprot_go >
    - GRAPH < GO >
  - Sub queries
    - Nothing
  - No. of federated queries: 0
  
Results:
| No. of GO<br> cellular components | No. of human DNA materials<br> relevant to cellular components (A) | No. of total<br> human DNA materials (B) | A/B | 
|:---:|:---:|:---:|:---:|
| 1,866 | 104,355 | 125,856 | 0.83 |   

