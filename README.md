# sim-plugin

> Applying SIM to LLM conversations through portable plugins and platform adapters.

This experimental project separates portable SIM conversation semantics from
platform-specific adapter mechanisms.

```text
SIM Conversation Specification
            |
     +------+------+
     |      |      |
   OpenAI Claude Gemini
     |      |      |
     +------+------+
            |
    Observed Behavior
```

- SIM semantics belong to the common specification.
- Platform-specific mechanisms belong to adapters.
- Differences in model and platform behavior are observed, not silently normalized.

The initial implementation target is OpenAI. The common specification does not
depend on any LLM platform.

See [the conversation specification](docs/conversation-spec.md) and
[OAMIU notes](docs/oamiu.md).
