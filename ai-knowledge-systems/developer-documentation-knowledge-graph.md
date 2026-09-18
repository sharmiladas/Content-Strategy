# Developer Documentation Knowledge-Graph Prototype

## The question

Developer documentation often spans concept guides, API references, tutorials, release notes, and troubleshooting content maintained by different teams. Links connect some of it, but many useful relationships remain implicit.

I built a proof of concept to explore whether explicit relationships could improve discovery and retrieval across those surfaces. This was an exploratory prototype, not production infrastructure.

## The content model

The prototype treated documents as more than pages with tags. It represented relationships such as:

- A procedure **implements** a concept
- A troubleshooting article **diagnoses** a known failure
- An API reference **belongs to** a product version
- A release note **changes** a behavior described elsewhere
- An example **demonstrates** a capability

Those distinctions matter because two pages can be textually similar without helping with the same task.

## The prototype workflow

1. Extract candidate entities and relationships from a bounded documentation set.
2. Compare them with the content model and flag uncertain matches.
3. Review high-impact or ambiguous relationships with a subject-matter expert.
4. Store the approved relationships with source and version information.
5. Test whether the graph improves related-content suggestions and retrieval results.

Tool connections were explored through the Model Context Protocol so search, retrieval, and validation could be tested as separate steps. Human review remained necessary for ambiguous technical relationships.

## What the prototype showed

The difficult work was not drawing a graph. It was defining what “related” meant for a developer task and deciding which relationships were worth maintaining. A smaller graph with clear semantics was more useful than a dense graph built from textual similarity alone.

## Next questions

- Which relationship types improve retrieval enough to justify their upkeep?
- How should version and product boundaries affect graph traversal?
- What confidence threshold should send a proposed relationship to review?
- How should corrections flow back to the source content?

[Back to AI knowledge systems](README.md) · [View the public portfolio](https://sharmiladas.github.io/)

