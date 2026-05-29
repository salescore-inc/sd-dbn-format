# SD-DBN Format

SD-DBN (Situated Dynamic Bayesian Network) is a domain-independent data format for representing how situated probabilistic beliefs change as new information is appended.

This repository contains the public format specification, JSON Schema entrypoint, and examples.

## Repository Structure

```text
sd-dbn-format/
  spec/
    sd-dbn.md
  schemas/
    sd-dbn.schema.json
  examples/
    valid/
      minimal.json
```

## Specification

- [SD-DBN Format Specification v3.0](spec/sd-dbn.md)

## Validation Scope

The JSON Schema validates static structure: required fields, primitive types, enums, event variants, time variants, and probability ranges.

Reference integrity and semantic conformance, such as relation endpoint constraints, `posterior` domain alignment, `current_beliefs` consistency, and revision policy checks, are validator responsibilities described in the specification.

## Status

This repository is the public home for the SD-DBN format. The schema should evolve with versioned compatibility rules.
