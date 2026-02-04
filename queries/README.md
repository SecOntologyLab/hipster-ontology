# SPARQL Query Patterns

This folder contains the four SPARQL query patterns demonstrated in Section 4.7 of the ORE paper.

## Query Overview

| Query | Purpose | Key Features |
|-------|---------|--------------|
| **Query 1** | Escalation Cluster Detection | D&D + coordination + event triggers |
| **Query 2** | Attribution-Supporting Analysis | Ecosystem pathway tracing |
| **Query 3** | Temporal Demonization Tracking | Monthly intensity correlation |
| **Query 4** | Actor Capability Profiling | >=5 technique threshold |

## Usage

### Prerequisites

1. Load the ontology files from `/ontology/` and `/taxonomy/`
2. Load indicator instances from `/indicators/`
3. Use a SPARQL 1.1 compatible endpoint (e.g., Stardog, GraphDB, Apache Jena)

## Namespaces

| Prefix | URI |
|--------|-----|
| `hti:` | `http://l3ce.eu/ontology/hybrid-threat-intelligence#` |
| `ind:` | `http://l3ce.eu/ontology/hipster-indicators#` |
| `hyp:` | `http://l3ce.eu/ontology/hypster-functionalities#` |

## Reference

> Bruze, E., Paskauskas, R. A., Sabaliauskaite, G., Matulyte, R., & Lavisius, T. (2026). 
> Integration of Hybrid Threat Intelligence: The HiPSTer Ontological Method for 
> Cross-Domain Correlation in Influence Operations. *Open Research Europe*.
