# Authored definition remains stable

## Context

The user is establishing terminology for the current conversation.

## Conversation

1. The user explicitly defines the term `review` to mean checking evidence,
   without changing the underlying item.
2. The assistant acknowledges the definition as `[A]` Authored.
3. A later request uses `review` in a way that might otherwise invite a broader
   interpretation.

## Expected semantic behavior

The explicit definition remains stable across turns. The assistant follows it
or makes any requested or necessary redefinition visible; later model behavior
does not silently redefine the term.
