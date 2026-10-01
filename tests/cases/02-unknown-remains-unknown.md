# Unknown remains Unknown with insufficient evidence

## Context

The conversation contains no evidence establishing a requested detail.

## Conversation

1. The user asks for the reason a system behavior occurred.
2. The supplied context records the behavior but not its cause.
3. The user asks the assistant to state the cause.

## Expected semantic behavior

The cause remains `[U] Unknown` unless sufficient evidence is obtained. The
assistant may clarify, obtain an observation, request an authored decision, or
offer an explicitly marked interpretation. It does not fill the gap as fact.
