# OAMIU labels

OAMIU is preferably pronounced **“oh-mew” / オーミュ**.

These labels distinguish the provenance or semantic status of a claim when that
distinction matters. Their exact SIM Foundation definitions are not established
in this repository; the descriptions below are therefore provisional and must
not be read as normative SIM semantics.

| Label | Name | Provisional meaning |
| --- | --- | --- |
| 🔵 `[O]` | Observed | Information presented as arising from observation or evidence. |
| 🟣 `[A]` | Authored | Information explicitly supplied, defined, or decided by an authoring participant. |
| 🟢 `[M]` | Model-derived | Information produced or derived by a model. |
| 🟡 `[I]` | Interpretation | A reading, inference, or framing that is distinct from observation. |
| ⚪ `[U]` | Unknown | Information not established by the available context or evidence. |

## Initial invariants

- Interpretation MUST NOT silently become Observation.
- Model-derived content MUST NOT silently become Observation.
- Unknown MUST NOT be silently filled as fact.
- Provenance distinctions should survive across conversation turns.

SIM Foundation is authoritative for refinements to these labels and invariants.
