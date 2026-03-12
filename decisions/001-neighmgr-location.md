# ADR-001: Neighsnoop Implemented in Zebra

## Status

Proposed

## Context

Neighbor snooping functionality needs access to:

- interface topology
- EVPN state
- neighbor cache

These are currently managed by Zebra.

Two main architectural approaches exist:

1. Implement neighsnoop inside Zebra
2. Implement neighsnoop as a separate daemon

## Decision

The initial implementation will integrate neighsnoop directly into Zebra.

## Consequences

### Positive

- Simpler implementation
- Direct access to EVPN data structures
- No new IPC mechanisms required

### Negative

- Increased Zebra complexity
- Harder to modularize later

