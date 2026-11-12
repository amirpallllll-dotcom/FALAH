# FALAH — Foundation

FALAH is a planned reference-guided 2D animation direction and production system.

**Current status:** planning/specification only. No animation engine or reference analyzer has been implemented yet.

## Goal
Given a new script, narration audio, and approved assets, FALAH should design scene-specific animation while preserving the visual and motion principles extracted from one chosen reference style.

## Non-negotiable principles
1. The reference teaches visual principles, not reusable scene choreography.
2. Every new scene gets its own action plan based on its narrative meaning.
3. Reusable rigs, joints, rendering primitives, camera math, and effect systems are allowed.
4. Reusing a complete action sequence is not the default; it requires a clear narrative reason.
5. Never claim a reference was fully analyzed unless the analysis report and coverage evidence exist.
6. Keep the existing What If `main`, Rewind, and CopyPaste untouched during FALAH development.
7. No paid APIs, subscriptions, or paid credits. Any optional service must be clearly marked as not part of the zero-budget baseline.

## Current development boundary
FALAH is being designed as an independent system. The existing Remotion project may later serve as a rendering backend, but FALAH must not become a collection of extra presets bolted onto What If.

See:
- [Architecture](docs/ARCHITECTURE.md)
- [Skill contract](docs/FALAH_SKILL.md)
- [Quality gates](docs/QUALITY_GATES.md)
- [Reference analysis format](docs/REFERENCE_ANALYSIS_SCHEMA.md)
