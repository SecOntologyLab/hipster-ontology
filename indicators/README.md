# Indicator Instance Data

This folder contains RDF/Turtle files defining the 143 threat indicator instances 
organised across 8 categories.

## File Overview

| File | Indicator Prefix | Count | Description |
|------|------------------|-------|-------------|
| `ind-ideology.ttl` | IDEO-* | ~20 | Ideology indicators (othering, restoration narratives) |
| `ind-fifthcolumn.ttl` | 5COL-* | ~40 | Fifth column indicators (attribution reversal) |
| `ind-conspiracy.ttl` | CONSP-* | ~20 | Conspiracy indicators (hidden enemy narratives) |
| `ind-rad-general.ttl` | RAD-GEN-* | ~25 | Radicalization general indicators |
| `ind-rad-person.ttl` | RAD-PERSON-* | ~15 | Radicalization person-level |
| `ind-rad-topic.ttl` | RAD-TOPIC-* | ~10 | Radicalization topic-level |
| `ind-rad-post.ttl` | RAD-POST-* | ~8 | Radicalization post-level |
| `ind-rad-event.ttl` | RAD-EVENT-* | ~5 | Radicalization event-level |

## Correspondence to Paper

These indicators map to:
- **Figure 3**: Example indicator instances
- **Section 3.4.3**: Indicator classes (IdeologyIndicator, FifthColumnIndicator, etc.)
- **Section 4**: Case study application

## Usage

Load these files alongside the core ontology (`/ontology/hipster-model.ttl`) and 
taxonomy (`/taxonomy/hyp-functionalities.ttl`) into your SPARQL endpoint.
