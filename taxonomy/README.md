# SKOS Capability Taxonomy

This folder contains the SKOS (Simple Knowledge Organization System) taxonomy 
defining the 12 functional domains and 143 detailed functionalities.

## The 12 Functional Domains

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

## File

| File | Description |
|------|-------------|
| `hyp-functionalities.ttl` | Complete SKOS taxonomy in Turtle format |

## Namespace

```
PREFIX hyp: <http://l3ce.eu/ontology/hypster-functionalities#>
```

## Usage

The taxonomy integrates with the OWL ontology via the `hyp:hasFunctionality` property,
linking indicator instances to their capability domain classifications.
