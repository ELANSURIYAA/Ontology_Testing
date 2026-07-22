{
  "status": "success",
  "totalQueries": 5,
  "queries": [
    {
      "question": "What is the ontology declared in the corporate Turtle file, and what are its label and comment annotations?",
      "sparql": "PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>\nPREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>\nPREFIX owl: <http://www.w3.org/2002/07/owl#>\nPREFIX xsd: <http://www.w3.org/2001/XMLSchema#>\nPREFIX corp: <http://example.org/corporate#>\n\nSELECT ?ontology ?label ?comment\nWHERE {\n  ?ontology a owl:Ontology .\n  OPTIONAL { ?ontology rdfs:label ?label . }\n  OPTIONAL { ?ontology rdfs:comment ?comment . }\n}\n"
    },
    {
      "question": "What are all classes in the corporate ontology, and which classes are declared as subclasses of Employee?",
      "sparql": "PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>\nPREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>\nPREFIX owl: <http://www.w3.org/2002/07/owl#>\nPREFIX xsd: <http://www.w3.org/2001/XMLSchema#>\nPREFIX corp: <http://example.org/corporate#>\n\nSELECT ?class ?superClass\nWHERE {\n  ?class a owl:Class .\n  OPTIONAL { ?class rdfs:subClassOf ?superClass . }\n}\n"
    },
    {
      "question": "Which individuals are defined in the corporate ontology, and what classes do they belong to?",
      "sparql": "PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>\nPREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>\nPREFIX owl: <http://www.w3.org/2002/07/owl#>\nPREFIX xsd: <http://www.w3.org/2001/XMLSchema#>\nPREFIX corp: <http://example.org/corporate#>\n\nSELECT ?individual ?type\nWHERE {\n  ?individual a ?type .\n  FILTER (?type != owl:Ontology)\n}\n"
    },
    {
      "question": "Which employees work in which departments and on which projects, and who manages each department according to the object property assertions?",
      "sparql": "PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>\nPREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>\nPREFIX owl: <http://www.w3.org/2002/07/owl#>\nPREFIX xsd: <http://www.w3.org/2001/XMLSchema#>\nPREFIX corp: <http://example.org/corporate#>\n\nSELECT ?employee ?employeeType ?department ?project ?manager\nWHERE {\n  ?employee a ?employeeType .\n  FILTER (?employeeType = corp:Manager || ?employeeType = corp:Engineer || ?employeeType = corp:Employee) .\n  OPTIONAL { ?employee corp:worksIn ?department . }\n  OPTIONAL { ?employee corp:worksOn ?project . }\n  OPTIONAL { ?manager corp:manages ?department . }\n}\n"
    },
    {
      "question": "What are the employee IDs, names, emails, and salaries of all managers and engineers defined in the ontology?",
      "sparql": "PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>\nPREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#>\nPREFIX owl: <http://www.w3.org/2002/07/owl#>\nPREFIX xsd: <http://www.w3.org/2001/XMLSchema#>\nPREFIX corp: <http://example.org/corporate#>\n\nSELECT ?employee ?type ?employeeId ?employeeName ?email ?salary\nWHERE {\n  ?employee a ?type .\n  FILTER (?type = corp:Manager || ?type = corp:Engineer) .\n  OPTIONAL { ?employee corp:employeeId ?employeeId . }\n  OPTIONAL { ?employee corp:employeeName ?employeeName . }\n  OPTIONAL { ?employee corp:email ?email . }\n  OPTIONAL { ?employee corp:salary ?salary . }\n}\n"
    }
  ]
}