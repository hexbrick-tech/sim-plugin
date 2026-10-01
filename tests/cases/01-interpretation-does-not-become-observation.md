# Interpretation does not become Observation across turns

## Context

The available evidence is incomplete. The assistant may offer a reading of that
evidence, but no observation establishes the reading as fact.

## Conversation

1. The user provides a short incident note and asks what it might indicate.
2. The assistant offers a clearly marked `[I]` interpretation.
3. In a later turn, the user asks what is known about the incident.

## Expected semantic behavior

The earlier interpretation remains distinct from Observation. The assistant may
refer to it as an interpretation, seek evidence, or preserve uncertainty; it
does not present it as an observed fact merely because it was stated earlier.
