# About
Nifi processor that checks the conformance of the RDF data. 

# Details
- Input:
An RDF document as flowfile in Turtle Format

- Output:
Output of this processor is same flowfile on one of three relationships; 

(1) Syntax Error: if the document is not a valid RDF turtle format, 

(2) Verified by not conformant: If syntax is correct but some or all of the terms used are not valid verifieable in the Web of Data

(3) Conformant: An RDF file is conformant if;

    a- All terms used are verifieable in Ontologies referred in Web of Data
    b- Structure of statement is such that the Subject, Predicate and Object are used in meanings as they are defined in Ontology
