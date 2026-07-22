{
  "ttlFile": "@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .\n@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .\n@prefix owl: <http://www.w3.org/2002/07/owl#> .\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n@prefix corp: <http://example.org/corporate#> .\n\n<http://example.org/corporate> a owl:Ontology ;\n    rdfs:label \"Corporate Organization Ontology\" ;\n    rdfs:comment \"Sample enterprise ontology for GraphDB and OWL to TTL conversion.\" .\n\ncorp:Company a owl:Class .\n\ncorp:Department a owl:Class .\n\ncorp:Employee a owl:Class .\n\ncorp:Manager a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Engineer a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Project a owl:Class .\n\ncorp:Client a owl:Class .\n\ncorp:Office a owl:Class .\n\ncorp:worksIn a owl:ObjectProperty .\ncorp:worksOn a owl:ObjectProperty .\ncorp:manages a owl:ObjectProperty .\ncorp:forClient a owl:ObjectProperty .\ncorp:locatedIn a owl:ObjectProperty .\n\ncorp:employeeId a owl:DatatypeProperty .\ncorp:employeeName a owl:DatatypeProperty .\ncorp:departmentName a owl:DatatypeProperty .\ncorp:projectName a owl:DatatypeProperty .\ncorp:clientName a owl:DatatypeProperty .\ncorp:officeLocation a owl:DatatypeProperty .\ncorp:salary a owl:DatatypeProperty .\ncorp:email a owl:DatatypeProperty .\n\ncorp:TechCorp a corp:Company .\n\ncorp:Engineering a corp:Department .\n\ncorp:Sales a corp:Department .\n\ncorp:HyderabadOffice a corp:Office .\n\ncorp:GlobalBank a corp:Client .\n\ncorp:AIPlatform a corp:Project .\n\ncorp:AliceJohnson a corp:Manager ;\n    corp:employeeId \"1001\" ;\n    corp:employeeName \"Alice Johnson\" ;\n    corp:email \"alice@techcorp.com\" ;\n    corp:salary \"95000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:manages corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n\ncorp:JohnSmith a corp:Engineer ;\n    corp:employeeId \"1002\" ;\n    corp:employeeName \"John Smith\" ;\n    corp:email \"john@techcorp.com\" ;\n    corp:salary \"72000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n",
  "status": "success"
}

----------

{
  "status": "success",
  "message": "TTL file successfully written to the GitHub repository.",
  "content": "@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .\n@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .\n@prefix owl: <http://www.w3.org/2002/07/owl#> .\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n@prefix corp: <http://example.org/corporate#> .\n\n<http://example.org/corporate> a owl:Ontology ;\n    rdfs:label \"Corporate Organization Ontology\" ;\n    rdfs:comment \"Sample enterprise ontology for GraphDB and OWL to TTL conversion.\" .\n\ncorp:Company a owl:Class .\n\ncorp:Department a owl:Class .\n\ncorp:Employee a owl:Class .\n\ncorp:Manager a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Engineer a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Project a owl:Class .\n\ncorp:Client a owl:Class .\n\ncorp:Office a owl:Class .\n\ncorp:worksIn a owl:ObjectProperty .\ncorp:worksOn a owl:ObjectProperty .\ncorp:manages a owl:ObjectProperty .\ncorp:forClient a owl:ObjectProperty .\ncorp:locatedIn a owl:ObjectProperty .\n\ncorp:employeeId a owl:DatatypeProperty .\ncorp:employeeName a owl:DatatypeProperty .\ncorp:departmentName a owl:DatatypeProperty .\ncorp:projectName a owl:DatatypeProperty .\ncorp:clientName a owl:DatatypeProperty .\ncorp:officeLocation a owl:DatatypeProperty .\ncorp:salary a owl:DatatypeProperty .\ncorp:email a owl:DatatypeProperty .\n\ncorp:TechCorp a corp:Company .\n\ncorp:Engineering a corp:Department .\n\ncorp:Sales a corp:Department .\n\ncorp:HyderabadOffice a corp:Office .\n\ncorp:GlobalBank a corp:Client .\n\ncorp:AIPlatform a corp:Project .\n\ncorp:AliceJohnson a corp:Manager ;\n    corp:employeeId \"1001\" ;\n    corp:employeeName \"Alice Johnson\" ;\n    corp:email \"alice@techcorp.com\" ;\n    corp:salary \"95000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:manages corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n\ncorp:JohnSmith a corp:Engineer ;\n    corp:employeeId \"1002\" ;\n    corp:employeeName \"John Smith\" ;\n    corp:email \"john@techcorp.com\" ;\n    corp:salary \"72000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n"
}

----------

{
  "status": "success",
  "content": "@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .\n@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .\n@prefix owl: <http://www.w3.org/2002/07/owl#> .\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n@prefix corp: <http://example.org/corporate#> .\n\n<http://example.org/corporate> a owl:Ontology ;\n    rdfs:label \"Corporate Organization Ontology\" ;\n    rdfs:comment \"Sample enterprise ontology for GraphDB and OWL to TTL conversion.\" .\n\ncorp:Company a owl:Class .\n\ncorp:Department a owl:Class .\n\ncorp:Employee a owl:Class .\n\ncorp:Manager a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Engineer a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Project a owl:Class .\n\ncorp:Client a owl:Class .\n\ncorp:Office a owl:Class .\n\ncorp:worksIn a owl:ObjectProperty .\ncorp:worksOn a owl:ObjectProperty .\ncorp:manages a owl:ObjectProperty .\ncorp:forClient a owl:ObjectProperty .\ncorp:locatedIn a owl:ObjectProperty .\n\ncorp:employeeId a owl:DatatypeProperty .\ncorp:employeeName a owl:DatatypeProperty .\ncorp:departmentName a owl:DatatypeProperty .\ncorp:projectName a owl:DatatypeProperty .\ncorp:clientName a owl:DatatypeProperty .\ncorp:officeLocation a owl:DatatypeProperty .\ncorp:salary a owl:DatatypeProperty .\ncorp:email a owl:DatatypeProperty .\n\ncorp:TechCorp a corp:Company .\n\ncorp:Engineering a corp:Department .\n\ncorp:Sales a corp:Department .\n\ncorp:HyderabadOffice a corp:Office .\n\ncorp:GlobalBank a corp:Client .\n\ncorp:AIPlatform a corp:Project .\n\ncorp:AliceJohnson a corp:Manager ;\n    corp:employeeId \"1001\" ;\n    corp:employeeName \"Alice Johnson\" ;\n    corp:email \"alice@techcorp.com\" ;\n    corp:salary \"95000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:manages corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n\ncorp:JohnSmith a corp:Engineer ;\n    corp:employeeId \"1002\" ;\n    corp:employeeName \"John Smith\" ;\n    corp:email \"john@techcorp.com\" ;\n    corp:salary \"72000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n"
}

----------

## Validation Summary

| Metric | Score | Reason |
|--------|------:|--------|
| Overall Validation Score | 100% | The Turtle ontology is a structurally and semantically faithful serialization of the source OWL ontology with no detected discrepancies. |
| Completeness | 100% | All ontology components (ontology IRI, prefixes, classes, properties, individuals, and assertions) present in the OWL source are represented in the Turtle output. |
| Accuracy | 100% | Class hierarchy, property types, annotations, and individual assertions in Turtle match the OWL source without namespace or datatype deviations. |
| Efficiency | 100% | The Turtle representation is concise, free of redundant triples, and uses standard prefixes and datatypes appropriately. |

## Completeness Findings

| Severity | Area | Issue Identified | Recommendation |
|----------|------|------------------|----------------|
| None | N/A | No completeness issues detected; all OWL entities and axioms appear in the Turtle ontology. | No action required. |

## Accuracy Findings

| Severity | Area | Issue Identified | Recommendation |
|----------|------|------------------|----------------|
| None | N/A | No accuracy issues detected; ontology declarations, namespaces, classes, properties, individuals, and annotations align with the OWL source. | No action required. |

## Efficiency Findings

| Severity | Area | Issue Identified | Recommendation |
|----------|------|------------------|----------------|
| None | N/A | No efficiency issues detected; the Turtle ontology is free of duplicate or superfluous triples and uses standard OWL/RDF constructs efficiently. | No action required. |