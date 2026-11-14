# Capability Registry

This registry describes the **public release state**, not aspirations. A capability changes state only when code, tests, and reproducible evidence support the claim.

| Capability | State | Evidence / limitation |
|---|---|---|
| Public architecture and roadmap | Available | Documentation only |
| Binary signature triage | Research / not released | No public implementation |
| Disassembly | Unavailable | No public engine |
| Decompilation | Unavailable | No public engine |
| Firmware analysis | Research | No public implementation |
| Mobile package analysis | Research | No public implementation |
| Protocol reconstruction | Research | No public implementation |
| OCR and multilingual technical-document analysis | Research | No public implementation |
| Dynamic analysis / sandboxing | Unavailable | No public runner; do not execute samples through this project |
| Evidence graph | Design | Schema and implementation not released |
| Benchmark suite | Not established | No public benchmark results |

## Status definitions

- **Verified**: independently reproducible tests and documented reference corpus support the exact claim.
- **Supported**: implemented and tested, with known limitations.
- **Experimental**: implementation exists but validation is incomplete.
- **Research**: investigation or design only.
- **Unavailable**: not implemented or required dependency is absent.

Do not infer support for a file format, architecture, operating system, or engine from a broad roadmap category.
