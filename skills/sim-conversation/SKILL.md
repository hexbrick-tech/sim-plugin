---
name: sim-conversation
description: Use when a conversation benefits from SIM-style provenance preservation, explicit Unknown handling, authored-definition stability, or semantic-boundary awareness.
---

# SIM Conversation

Apply the repository's SIM Conversation Specification to the current conversation.

## Source of truth

Treat these repository documents as the semantic source:

- `docs/conversation-spec.md`
- `docs/oamiu.md`

Do not invent normative SIM semantics beyond those documents. If the source leaves something unspecified, preserve that uncertainty rather than silently completing it.

## Behavior

- Preserve provenance across turns.
- Do not silently turn Interpretation into Observation.
- Do not silently turn Model-derived content into Observation.
- Do not silently fill Unknown as fact.
- Preserve explicitly authored definitions and decisions unless the user revises them.
- When the interaction materially changes activity or purpose, make the semantic-boundary change visible instead of silently changing modes.
- Use visible OAMIU labels only when the provenance distinction materially helps the conversation; do not label every sentence by default.

## Unknown handling

When information is not established, keep it Unknown unless the conversation establishes it through an observation, an authored decision, or an explicitly marked interpretation.

Possible responses to Unknown include asking for clarification, requesting observation, requesting or establishing an authored decision, forming an explicitly marked interpretation, or preserving the Unknown. These actions are provisional guidance, not a formal state machine.

## Constraint

This skill is a platform adapter for the repository's conversation semantics. It must not redefine the common SIM specification.
