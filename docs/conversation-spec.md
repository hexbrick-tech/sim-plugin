# SIM Conversation Specification

**Draft 0.1**

## Purpose

This draft describes a minimal, platform-independent view of what it means for
an assistant to participate in a conversation using SIM principles. It records
only behavior identified for this repository so far. SIM Foundation is the
authoritative source for SIM; unspecified matters remain open.

## OAMIU classification

Relevant claims may be distinguished using OAMIU when provenance matters. Normal
conversation does not require every sentence to carry a visible label.

The labels and their repository-local provisional descriptions are in
[OAMIU labels](oamiu.md). This draft does not define a formal transition state
machine for them.

## Provenance preservation

Information should retain its semantic and provenance status across turns. A
previous Interpretation or Model-derived statement must not later be treated as
an Observation merely because it appeared earlier in the conversation.

## Unknown preservation and handling

`[U] Unknown` is a valid state, not merely a missing field for the model to
complete automatically.

Where useful, an Unknown may lead to one or more of the following provisional
actions:

- clarify with the user;
- obtain an observation;
- request or establish an authored decision;
- form an explicitly marked interpretation; or
- preserve the Unknown.

This vocabulary is provisional. It is not a formal state machine.

## Semantic boundary awareness

When a conversation begins performing a materially different activity from the
one currently established, the assistant should make that boundary change
visible rather than silently changing the nature of the interaction.

For example, an advisory conversation that drifts into performing the underlying
research itself may represent a semantic-boundary change. This draft does not
attempt to enumerate all possible boundaries.

## Progressive stabilization

Conversation may progressively turn ambiguous material into explicit authored
definitions or decisions. Once something has been explicitly authored, later
model behavior should not silently redefine it.

## Open scope

This draft does not specify platform mechanisms, APIs, classifiers, automated
evaluation, or runtime behavior. Those areas should evolve from observed plugin
behavior rather than from an attempt to fully specify SIM conversation behavior
at this stage.
