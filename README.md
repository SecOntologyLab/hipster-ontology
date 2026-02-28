# Hybrid-Threat Intelligence: The HIPSTer Ontological Framework

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Ontology for hybrid-threat intelligence (OSINT - SoCMINT - NLP)**

This repository contains the **research artefacts** and **technical validation results** for the HIPSTer (Hybrid Information Psychological Societal Threats) project.

## Publications

This framework is documented in:

1. **Paskauskas, R. A., Bružė, E., Sabaliauskaitė, G., Matulytė, R., & Lavišius, T.** (2026). Hybrid-Threat Intelligence: A Critical Review of Semantic Integration Challenges and the HIPSTer Ontological Framework. *Journal of Intelligent Communication* (forthcoming).

2. **Bružė, E., Paskauskas, R. A., Sabaliauskaitė, G., Matulytė, R., & Lavišius, T.** (2026). Integration of Hybrid Threat Intelligence: The HiPSTer Ontological Method for Cross-Domain Correlation in Influence Operations. *Open Research Europe* (forthcoming).

## Repository Contents

### `/ontology/` - Core OWL Ontology

| File | Description |
|------|-------------|
| `hipster-model.ttl` | Core OWL ontology defining classes and object properties |
| `hipster-subset-viz.ttl` | Subset optimised for visualisation |
| `ChCOLD_validation_results.txt` | Chinese COLD dataset validation results |

### `/taxonomy/` - SKOS Capability Taxonomy

| File | Description |
|------|-------------|
| `hyp-functionalities.ttl` | SKOS taxonomy covering 12 functional domains and 143 detailed functionalities |

**The 12 Functional Domains:**
1. Communication Metadata
2. Language and Phrasing
3. Symbolism and Imagery
4. Narratives and Storytelling
5. Community and Engagement Patterns
6. Behavioural Patterns and Activity Trends
7. Visual and Aesthetic Cues
8. Cultural References and Symbolic Associations
9. Social Media Metadata and Geolocation
10. Content Structure and Framing Strategies
11. **Dehumanization and Demonization** (primary focus of case study)
12. Anomalies and Psychological Patterns

### `/indicators/` - Indicator Instance Data

| File | Indicator Class | Description |
|------|-----------------|-------------|
| `ind-ideology.ttl` | IDEO-* | Ideology indicators (othering, restoration narratives) |
| `ind-fifthcolumn.ttl` | 5COL-* | Fifth column indicators (attribution reversal, delegitimisation) |
| `ind-conspiracy.ttl` | CONSP-* | Conspiracy indicators (hidden enemy, existential threat) |
| `ind-rad-general.ttl` | RAD-GEN-* | Radicalization general indicators |
| `ind-rad-person.ttl` | RAD-PERSON-* | Radicalization person-level indicators |
| `ind-rad-topic.ttl` | RAD-TOPIC-* | Radicalization topic-level indicators |
| `ind-rad-post.ttl` | RAD-POST-* | Radicalization post-level indicators |
| `ind-rad-event.ttl` | RAD-EVENT-* | Radicalization event-level indicators |

### `/queries/` - SPARQL Query Patterns

| File | Purpose |
|------|---------|
| `query1-escalation-cluster.sparql` | Detect D&D campaigns with coordination signals near event triggers |
| `query2-attribution-pattern.sparql` | Trace ecosystem pathways from state actors through proxy outlets |
| `query3-temporal-tracking.sparql` | Track demonization intensity over time against target groups |
| `query4-actor-profiling.sparql` | Identify actors employing 5+ distinct D&D techniques |

### `/visualisations/` - Interactive Demonstrations

| File | Content | Notes |
|------|---------|-------|
| `ontology-network.html` | Core ontology structure | Corresponds to Figure 1 |
| `ontology-demo.html` | Russia-Ukraine case study | Demonstrates 5 of 7 indicators from Figure 3 |
| `sparql-demo.html` | Query demonstrations | Simplified versions for accessibility |

**Note:** The interactive SPARQL demos are illustrative. For formal query specifications, see `/queries/`.
## 🔬 Live Interactive Demos

> Click any demo below to launch directly in your browser — no installation required.

| Demo | Description |
|------|-------------|
| [🌐 Ontology Explorer](https://secontologylab.github.io/hipster-ontology/visualisations/ontology-demo.html) | Browse the full HIPSTer ontology class hierarchy and class definitions |
| [🕸️ Ontology Network](https://secontologylab.github.io/hipster-ontology/visualisations/ontology-network.html) | Interactive node-link visualisation of semantic relationships across hybrid threat domains |
| [🔍 SPARQL Query Demo](https://secontologylab.github.io/hipster-ontology/visualisations/sparql-demo.html) | Run live SPARQL queries against the HIPSTer ontology and explore inference results |

### `/data/` - Assessment Data

Comparative assessment data underlying Tables 1-2 in the ORE paper.

### `/docs/` - Documentation

Extended framework documentation and methodology notes.

## Related Resources

- **ML/NLP Validation Pipeline (KTU):** https://github.com/evavaic/KTU-Misijos-HIPSTer
- **5G Hybrid Threats Ontology:** https://purl.org/5g-hybrid-threats

## Quick Start

### Load the Ontology

Import `ontology/hipster-model.ttl` into [Protege](https://protege.stanford.edu/) or any OWL-compatible editor.

### Run SPARQL Queries

Load the ontology and indicator files into [Stardog Cloud](https://cloud.stardog.com/) or another SPARQL endpoint, then execute queries from `/queries/`.

### Explore the Taxonomy

The SKOS taxonomy in `taxonomy/hyp-functionalities.ttl` can be browsed in any RDF viewer or imported into knowledge management tools.

## Namespaces

| Prefix | URI |
|--------|-----|
| `hti:` | `http://l3ce.eu/ontology/hybrid-threat-intelligence#` |
| `ind:` | `http://l3ce.eu/ontology/hipster-indicators#` |
| `hyp:` | `http://l3ce.eu/ontology/hypster-functionalities#` |

## Citation

```bibtex
@article{bruze2026hipster,
  title={Integration of Hybrid Threat Intelligence: The HiPSTer Ontological Method for Cross-Domain Correlation in Influence Operations},
  author={Bruze, Evaldas and Paskauskas, R. Andrew and Sabaliauskaite, Giedre and Matulyte, Raminta and Lavisius, Tomas},
  journal={Open Research Europe},
  year={2026}
}
```

## Acknowledgements

This research was prepared as part of the project "Implementation of Mission-Based Science and Innovation Programs" (Project No. 02-002-P-0001), financed by the European Union through the Recovery and Resilience Facility (2021-2027 programming period, New Generation Lithuania plan), and co-funded by the state budget of the Republic of Lithuania administered via the Research Council of Lithuania.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
