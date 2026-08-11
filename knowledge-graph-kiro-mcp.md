---
title: "Building a Knowledge Graph for Developer Documentation with Kiro and MCP"
published: false
description: "Using agentic tooling — Kiro, MCP, and reasoning loops — to build a knowledge graph that plans, executes, and reviews its own content work."
tags: ai, agenticai, documentation, mcp
series: "Content Strategy in the AI Era"
---

## The Problem

At a large-scale developer platform organization, developer documentation spans five distinct surfaces, each maintained by different teams on different cadences. Related content — a concept explained in one place, a reference for it somewhere else, a troubleshooting guide referencing both — often isn't connected at all. That hurts discoverability for human readers, and it's a worse problem for AI-assisted retrieval: an AI agent trying to answer a question can only be as good as the connections in the underlying content.

## What I Built

As Senior Technical Program Manager, Content Strategy and Developer Experience, I built a **knowledge graph for developer documentation** using **Kiro**, linking related content across surfaces to improve discoverability and support AI-assisted retrieval.

The architecture behind it:

- **Structured content models** — the documentation isn't just tagged, it's modeled, so relationships between concepts, references, and procedures are explicit rather than implied by folder structure or hyperlinks.
- **Reasoning loops** that allow the system to evaluate content relationships, not just index them — asking whether two pieces of content are actually related, not just textually similar.
- **Tool integrations via the Model Context Protocol (MCP)**, connecting the reasoning system to the actual content tooling it needs to act on — search, retrieval, validation.

Together, these let the system **plan, execute, review, and optimize content lifecycles with minimal step-by-step human intervention** — moving from a static, human-curated graph toward one that can maintain and improve itself as documentation changes.

## Why This Is a Content Strategy Problem, Not Just an Engineering One

It would be easy to treat a knowledge graph as a purely technical build. The harder, more strategic part was defining what "related" should mean for documentation specifically — what relationships actually help a developer or an AI agent, versus relationships that are technically true but practically useless. That's a content and information architecture judgment, encoded into a system that then applies it at scale.

## Impact

- Improved discoverability of related content across five previously disconnected documentation surfaces
- Laid the technical and architectural groundwork for AI-assisted retrieval across a large developer documentation portfolio
- Established a working pattern for agentic content operations — systems that don't just store content, but reason about and act on it

## Tools

Kiro, Model Context Protocol (MCP), structured content modeling, agent architectures

---

*This is part of a series on content strategy in the AI era.*
