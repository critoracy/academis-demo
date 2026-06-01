---
title: "Open Urban Documentation Initiative"
subtitle: "Building a publicly accessible record of informal housing in post-industrial cities"
publishDate: 2025-10-18
lead: "A two-year project to document, archive, and publish the built fabric of informal housing settlements in three European post-industrial cities — creating a resource that is free, searchable, and maintained by the communities it documents."
author: "thomas-vance"
cover: "cover.png"
tags: ["urbanism", "open data", "architecture", "documentation", "project"]
role: "Project Lead & Technical Architect"
organization: "Urban Commons Research Collaborative"
period: "2024 – 2026"
params:
  toc: false
---

## Why this project exists

Informal housing — self-built, incrementally expanded, legally ambiguous — is the dominant form of housing for a significant portion of the urban population globally, including in cities that do not normally appear in discussions of the "global south." Post-industrial cities in Eastern and Southern Europe have substantial informal settlements whose built history is almost entirely undocumented in any accessible form.

This creates a specific kind of institutional blindness: planning authorities make decisions about these areas based on maps that do not reflect what is actually built; residents cannot access formal credit because their homes do not appear in cadastral records; and the accumulated knowledge of how communities have solved housing problems with minimal resources is lost when settlements are demolished or regularised.

## What we built

{{< cols left="60" right="40" >}}
{{< col >}}
The project produced three connected outputs:

**A photographic and technical archive** — 4,800 buildings across three cities documented with standardised photography, measured drawings where accessible, and structured metadata (construction materials, approximate date, modifications over time).

**A public web platform** — searchable, map-based, downloadable under Creative Commons. All data available via API for research use.

**A community annotation tool** — allowing residents to add contextual information, correct errors, and flag buildings at risk. Built on a simple mobile-first interface after testing showed that complex GIS tools created barriers for non-technical contributors.
{{< /col >}}
{{< col >}}
{{< box variant="highlight" >}}
**Project numbers:**
- 3 cities
- 4,800 buildings documented
- 23 community contributors trained
- 6 research teams currently using the dataset
- CC BY 4.0 licence throughout
{{< /box >}}
{{< /col >}}
{{< /cols >}}

## Technical architecture

The platform runs entirely on static-site infrastructure — a deliberate choice for long-term sustainability. Previous urban documentation projects have failed when grant funding ended and hosting costs could not be covered; a statically generated site can be archived and mirrored at near-zero cost.

Documentation data is stored as structured JSON and rendered through a client-side search and map interface (Leaflet + Lunr). The annotation tool uses a lightweight serverless backend for write operations, with daily exports to the main static dataset.

## What we learned

**Community engagement is not optional.** The first six months of the project used a traditional top-down documentation methodology. The data we collected was accurate but shallow — it documented facades without understanding histories. Once we shifted to training community members to lead documentation in their own areas, both the volume and the quality of the archive improved substantially.

**Legal clarity matters early.** Informal housing sits in a complicated legal position. We spent more time than anticipated on the licensing and consent framework, including situations where documenting a building could, in principle, affect its legal status. A working protocol with a legal aid organisation was necessary before fieldwork could proceed at scale.

**The platform is now maintained by the communities it documents** — an outcome that was the goal from the start but that required investing significantly in training and governance structures rather than just the technical build.

## Documentation and replication

Full project documentation, including the technical architecture, field methodology, and community training materials, is available on the project repository under CC BY 4.0. The platform codebase is MIT licensed.

{{< btn href="https://example.com/oud-project" variant="primary" >}}View project site{{< /btn >}}
{{< btn href="https://github.com/example/oud-platform" variant="secondary" >}}Source code{{< /btn >}}
