{
  "status": "success",
  "content": "@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .\n@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .\n@prefix owl: <http://www.w3.org/2002/07/owl#> .\n@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .\n@prefix corp: <http://example.org/corporate#> .\n\n<http://example.org/corporate> a owl:Ontology ;\n    rdfs:label \"Corporate Organization Ontology\" ;\n    rdfs:comment \"Sample enterprise ontology for GraphDB and OWL to TTL conversion.\" .\n\ncorp:Company a owl:Class .\n\ncorp:Department a owl:Class .\n\ncorp:Employee a owl:Class .\n\ncorp:Manager a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Engineer a owl:Class ;\n    rdfs:subClassOf corp:Employee .\n\ncorp:Project a owl:Class .\n\ncorp:Client a owl:Class .\n\ncorp:Office a owl:Class .\n\ncorp:worksIn a owl:ObjectProperty .\ncorp:worksOn a owl:ObjectProperty .\ncorp:manages a owl:ObjectProperty .\ncorp:forClient a owl:ObjectProperty .\ncorp:locatedIn a owl:ObjectProperty .\n\ncorp:employeeId a owl:DatatypeProperty .\ncorp:employeeName a owl:DatatypeProperty .\ncorp:departmentName a owl:DatatypeProperty .\ncorp:projectName a owl:DatatypeProperty .\ncorp:clientName a owl:DatatypeProperty .\ncorp:officeLocation a owl:DatatypeProperty .\ncorp:salary a owl:DatatypeProperty .\ncorp:email a owl:DatatypeProperty .\n\ncorp:TechCorp a corp:Company .\n\ncorp:Engineering a corp:Department .\n\ncorp:Sales a corp:Department .\n\ncorp:HyderabadOffice a corp:Office .\n\ncorp:GlobalBank a corp:Client .\n\ncorp:AIPlatform a corp:Project .\n\ncorp:AliceJohnson a corp:Manager ;\n    corp:employeeId \"1001\" ;\n    corp:employeeName \"Alice Johnson\" ;\n    corp:email \"alice@techcorp.com\" ;\n    corp:salary \"95000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:manages corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n\ncorp:JohnSmith a corp:Engineer ;\n    corp:employeeId \"1002\" ;\n    corp:employeeName \"John Smith\" ;\n    corp:email \"john@techcorp.com\" ;\n    corp:salary \"72000\"^^<http://www.w3.org/2001/XMLSchema#decimal> ;\n    corp:worksIn corp:Engineering ;\n    corp:worksOn corp:AIPlatform .\n"
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
| Overall Validation Score | 99% | The Turtle ontology is syntactically valid and matches the source OWL ontology across ontology declaration, namespaces, classes, properties, individuals, and assertions with no detected loss or distortion of content. |
| Completeness | 100% | All ontology components present in the OWL source (ontology IRI, prefixes, classes, subclass axioms, object/datatype properties, individuals, annotations, and property assertions) are represented in the Turtle output. |
| Accuracy | 99% | Entity IRIs, class hierarchies, property types, and assertion structures are correctly preserved; the only minor deviation is the explicit use of xsd:decimal via full IRI in salary literals, which is semantically equivalent but not prefix-optimized. |
| Efficiency | 99% | The Turtle serialization is compact, free of redundant or duplicate triples, and uses consistent prefixes; minor efficiency improvement is possible by using the xsd prefix instead of full datatype IRIs in salary literals. |

## Completeness Findings

| Severity | Area | Issue Identified | Recommendation |
|----------|------|------------------|----------------|
| None | Ontology declaration | No missing ontology IRI or ontology-level annotations; Turtle ontology includes rdfs:label and rdfs:comment matching the source OWL. | No action required. |
| None | Namespaces | All standard namespaces (rdf, rdfs, owl, xsd) and the corporate namespace (corp) are present and consistent with the source OWL ontology. | No action required. |
| None | Classes | All corporate classes (Company, Department, Employee, Manager, Engineer, Project, Client, Office) from the OWL ontology are present in the Turtle file. | No action required. |
| None | Subclass relationships | Subclass axioms (Manager ⊑ Employee, Engineer ⊑ Employee) are fully present and correctly represented via rdfs:subClassOf. | No action required. |
| None | Object properties | All object properties (worksIn, worksOn, manages, forClient, locatedIn) appear in the Turtle ontology as owl:ObjectProperty instances. | No action required. |
| None | Datatype properties | All datatype properties (employeeId, employeeName, departmentName, projectName, clientName, officeLocation, salary, email) are present as owl:DatatypeProperty instances. | No action required. |
| None | Individuals | All individuals in the source OWL (TechCorp, Engineering, Sales, HyderabadOffice, GlobalBank, AIPlatform, AliceJohnson, JohnSmith) are present with their correct rdf:type assertions. | No action required. |
| None | Annotations | Ontology-level annotations (label, comment) are preserved; no missing annotation statements were detected. | No action required. |
| None | Object property assertions | All object property assertions (worksIn, worksOn, manages) for AliceJohnson and JohnSmith are present and match the OWL source. | No action required. |
| None | Datatype property assertions | All datatype assertions (employeeId, employeeName, email, salary) for AliceJohnson and JohnSmith are present with appropriate literal values and datatypes. | No action required. |

## Accuracy Findings

| Severity | Area | Issue Identified | Recommendation |
|----------|------|------------------|----------------|
| Low | Datatype representation | Salary literals use the full IRI `<http://www.w3.org/2001/XMLSchema#decimal>` instead of the declared `xsd:` prefix, which is semantically equivalent but slightly inconsistent with prefix usage elsewhere. | Normalize salary datatype usage to `\"...\"^^xsd:decimal` for consistency with the declared `xsd` prefix while keeping the datatype identical. |
| None | Class and subclass mappings | Class IRIs and subclass relations match the OWL source with no incorrect or missing mappings. | No action required. |
| None | Object property mappings | Object properties and their assertion targets are accurately mapped; domains/ranges implied by usage align with the source. | No action required. |
| None | Datatype property mappings | Datatype properties and their associated literals correctly reflect the OWL ontology, including identifiers, names, emails, and salaries. | No action required. |
| None | Individual IRIs | Individual IRIs and their types are preserved without renaming or structural changes that could affect referential integrity. | No action required. |

## Efficiency Findings

| Severity | Area | Issue Identified | Recommendation |
|----------|------|------------------|----------------|
| Low | Datatype prefix usage | Use of full datatype IRIs for salary values instead of the existing `xsd` prefix slightly reduces serialization conciseness and prefix reuse. | Replace full datatype IRIs with `xsd:decimal` to improve readability and prefix efficiency while maintaining semantic equivalence. |
| None | Redundancy in triples | No duplicate or redundant class, property, or assertion triples were detected; each statement is necessary for the described domain model. | No action required. |
| None | Namespace configuration | Prefix declarations are minimal and sufficient; no unused or superfluous prefixes that would affect parsing or readability were found. | No action required. |
| None | Structural organization | The ordering and grouping of ontology elements (classes, properties, individuals) support efficient parsing and maintenance, with no structural inefficiencies identified. | No action required. |