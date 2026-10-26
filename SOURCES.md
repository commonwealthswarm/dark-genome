# Sources

Every real source this project uses or plans to use is listed here with its terms. A source is only used for research
work after the Night Shift operator registers a curated source entry for it. Nothing listed below has been analysed.

## Inventory and blockers

Real-data state: **pending_source_entry** (gate: curated source entry).

ENCODE v4 GRCh38 cCRE annotations file ENCFF796PQR from analysis ENCAN752RNF (released data, attribution required). Real work uses only the reviewed 100-annotation chr1 sample, as bounded unit tasks the Worker generates from that exact registered file, and only while it is registered. Imported candidate regions are annotations, not analysed regions and not functional proof.

Inventory:
- ENCFF796PQR (analysis ENCAN752RNF), ENCODE released v4, GRCh38 cCRE annotations: first 100 chr1 annotations inside chr1:0-1,000,000

Blockers:
- Real-data tasks exist only while the reviewed chr1 sample is registered as a curated source with its exact hash.

## Rules

- Do not commit source data files. Records point to sources; they do not copy them (a test enforces this).
- Records built from a description alone are `unverified` and carry no hash.
- A source whose redistribution terms are restricted or unresolved is never marked publishable.
