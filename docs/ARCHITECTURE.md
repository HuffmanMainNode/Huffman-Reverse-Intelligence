# HRI Public Architecture

## Design goals

HRI aims to be a local-first, offline-capable, modular reverse-engineering workbench. Its core should orchestrate independently maintained specialist engines, preserve evidence provenance, and expose the same stable analysis contracts to a CLI and optional desktop interface.

## Proposed layers

1. Artifact intake and immutable identification.
2. Format, architecture, and container identification.
3. Specialist analysis adapters for binaries, source, firmware, mobile, protocols, documents, and hardware references.
4. Evidence graph for observations, derived facts, hypotheses, contradictions, and provenance.
5. Reconstruction models for structures, control/data flow, formats, and protocol state machines.
6. Verification through golden corpora, differential testing, round trips, and independent review.
7. CLI and optional desktop interfaces.

## Adapter requirements

Every adapter should declare an ID, version, supported inputs, platform requirements, external dependencies, license, network behavior, execution behavior, resource limits, output schema, and known limitations. Optional engines must be replaceable. Missing dependencies must be reported as unavailable, not silently skipped.

## Evidence requirements

A complete evidence record is expected to identify the input digest, operation, tool and adapter versions, configuration, timestamp, output digest, warnings, and whether a claim is observed, derived, or hypothesized. Confidence must be tied to a stated method, not generated as an unsupported number.

## Safety boundary

Parsing is not execution. Dynamic analysis, when designed, must use disposable isolation with explicit consent, constrained resources, controlled networking, no host credentials, and teardown verification. The public project has not implemented that runner.
