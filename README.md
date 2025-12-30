# hipster-ontology
Ontology for hybrid-threat intelligence (OSINT · SoCMINT · NLP)

Hybrid-Threat Intelligence: The HIPSTer Ontological Framework
This repository contains the research artefacts and technical validation results for the manuscript:
"Hybrid-Threat Intelligence: A Critical Review of Semantic Integration Challenges and the HIPSTer Ontological Framework".
This project is a work-in-progress initiative persistently developed by the Security Research Laboratory, Mykolas Romeris University (MRU) in collaboration with the Lithuanian Cybercrime Centre of Excellence (L3CE).
Project Overview
The HIPSTer (Hybrid Information Psychological Societal Threats handling system) framework addresses the "semantic gap" in current defensive systems by providing an ontology-driven architecture for multi-domain threat correlation. It integrates OWL threat modeling and SKOS taxonomies to enable formal reasoning over disparate data streams.
Technical Validation (TRL 4)
The initiative has successfully reached Technology Readiness Level 4 (Laboratory Validation).
Key Performance Benchmarks
Experimental validation demonstrates high predictive accuracy and computational efficiency using high-efficiency semantic vectors and SPARQL (Protocol and RDF Query Language):
.	Chinese Offensive Language Detection (COLD): Achieved 86% Accuracy and an AUC-ROC of 0.931.
.	Classification Reliability: Demonstrated a Cohen’s Kappa of 0.72 for Mandarin-based threat indicators.
.	Operational Efficiency: Processed adversarial benchmarks in under 3 minutes (total wall time for cross-validation ~10 minutes) on standard Google Colab (Tesla T4 GPU) cloud infrastructure.
Repository Structure
.	/ontology: Contains the core research artefacts, including:
o	operational_query_example.rq: The formal SPARQL implementation for cross-domain reasoning.
o	ChCOLD_validation_results.txt: Raw cross-validation logs for the Chinese linguistic extension 
.	/docs: Expert-based evaluation methodology and functional requirements framework.
.	/data: OSINT tool competitive analysis and SKOS taxonomy mapping data.
Institutional Context & Funding
This research is part of the project “Implementation of Mission-Based Science and Innovation Programs” (Project No. 02-002-P-0001). It is financed by the European Union through the Recovery and Resilience Facility and co-funded by the Republic of Lithuania via the Research Council of Lithuania.
Foundational machine learning pipelines for European linguistic contexts (English, Lithuanian, Russian) are based on the KTU-Misijos-HIPSTer repository.

