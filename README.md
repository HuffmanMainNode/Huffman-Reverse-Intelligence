# Huffman Reverse Intelligence (HRI)

<sub>**UNDER CONSTRUCTION · PRE-ALPHA · NOT A RELEASE**</sub>

Huffman Reverse Intelligence is an open-source initiative to build a local-first, extensible, evidence-driven workbench for reverse engineering and technical analysis of systems and artifacts that users are authorized to examine.

The long-term research scope includes source repositories, native binaries, libraries, mobile packages, firmware, file formats, network protocols, technical documents, and hardware references. Universal compatibility is an architectural objective, not a current capability claim.

## Current status

This public repository is the project entry point and public design record. **It does not currently contain a usable reverse-engineering engine or a production-ready application.** The private engineering workspace is maintained separately and is not mirrored here automatically.

| Capability area | Public project status |
|---|---|
| Binary identification and disassembly | Research / not released |
| Decompilation and structural recovery | Research / not released |
| Firmware and mobile analysis | Research / not released |
| Protocol and file-format reconstruction | Research / not released |
| Dynamic analysis and sandboxing | Unavailable / not released |
| Evidence provenance and reproducibility | Design in progress |
| CLI and desktop interfaces | Not released |

## Design commitments

- Local-first and usable without a mandatory hosted service.
- Optional, replaceable specialist engines rather than a single-vendor dependency.
- Evidence provenance, reproducible outputs, and explicit capability limitations.
- Safe defaults: no automatic execution of inspected artifacts and no implicit artifact uploads.
- Open development with dependency, licensing, and security review.
- No fabricated benchmarks, unsupported compatibility claims, or unverified completion statements.

## Planned technical domains

1. Source and repository architecture, dependency and build analysis.
2. Executables, shared libraries, object formats, disassembly, and decompilation.
3. Mobile application packages and native components.
4. Firmware, bootloaders, embedded filesystems, and device interfaces.
5. Network protocols, APIs, serialization, and state-machine inference.
6. Binary file formats, containers, compression, and data structures.
7. Technical documents, manuals, schematics, and cross-domain evidence correlation.

See [ARCHITECTURE.md](docs/ARCHITECTURE.md), [CAPABILITIES.md](docs/CAPABILITIES.md), and [ROADMAP.md](docs/ROADMAP.md).

## Use and authorization

Use reverse-engineering tools only within the scope of applicable law and valid authorization. Public availability does not automatically grant permission to bypass technical controls, redistribute protected material, or process private data. Read [ACCEPTABLE_USE.md](ACCEPTABLE_USE.md) and [SECURITY.md](SECURITY.md). These documents are not legal advice.

## Licensing

**No open-source license has been selected or granted yet.** Until a complete license and third-party dependency review are published, do not assume permission to reuse, modify, or redistribute project code. See [LICENSE-PENDING.md](LICENSE-PENDING.md).

## Contributing

Early contributions should focus on architecture review, threat modeling, reproducibility, test design, documentation corrections, and independently verifiable implementations. Read [CONTRIBUTING.md](CONTRIBUTING.md).

## Release gate

No release will be declared until supported capabilities have reproducible tests, dependencies and licenses are reviewed, security boundaries are documented, and all required CI checks pass. The project will publish known limitations and unsupported cases alongside capabilities.
