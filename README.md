RLOG
====

RLOG - an RDF Logging Ontology and its Bindings

##TODO 
- move RLOG classes from /home/sebastian/svn/RLOG/maven/jena/src/main/java/org/nlp2rdf/core/vocab to their own module maven/vocab


## RLOG - an RDF Logging Ontolog
The ontology is hosted at:
http://persistence.uni-leipzig.org/nlp2rdf/ontologies/rlog#

and maintained via:
https://github.com/NLP2RDF/persistence.uni-leipzig.org

The main rationale for this step is that persistent hosting and debugging infrastructure is already in place at NIF/NLP2RDF project. No need to duplicate this. You can send pull requests and get access there as for editing the ontology (if necessary). 

## How to contribute

You can contribute issues here:
https://github.com/AKSW/RLOG/issues

We are always happy about new bindings and improvements. 

If you have any questions, please write an issue as well. 

##License
All open and free. Apache is preferred. Please drop us a note, if you need to re-license.

## Binding generation

Most of the bindings are generated directly from the ontology. Please have a look at the tools folder. There is a class in there which is called "Generate.java", which calls the Velocity templates in tools/src/main/resource/ to generate the bindings


'''bash
cd tools
#for help
mvn exec:java -e  -Dexec.mainClass="org.nlp2rdf.tools.Generate" -Dexec.args="-h" 
#to run
mvn exec:java -e  -Dexec.mainClass="org.nlp2rdf.tools.Generate" -Dexec.args="-t DatatypeProperties -f ../core/nif/src/main/java/org/nlp2rdf/core/vocab/RLOGDatatypeProperties.java -o http://persistence.uni-leipzig.org/nlp2rdf/ontologies/rlog#"
'''

## Current Bindings

### Java / Maven

TODO

### Jena + SLF4J





