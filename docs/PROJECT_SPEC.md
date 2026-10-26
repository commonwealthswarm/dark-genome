# Project specification: Mapping the dark genome

project-id: dark-genome
mission: dark-genome
plan: experiment-plan-v1:dark-genome:7e4edf18

## Purpose

Open software and sourced evidence records for judging which non-coding human DNA regions deserve follow-up. Computation gives clues, not biological confirmation. No region has been analysed yet.

## Work modes

- **Software on synthetic fixtures**: ready_when_repo_verified. Interval, evidence-ledger and Atlas-data code tested on synthetic GRCh38-style coordinates.
- **Source audit (documentary records)**: ready_when_repo_verified. Provenance records for the ENCODE release, from facts stated in the task only.
- **Real-data research**: pending_source_entry. ENCODE v4 GRCh38 cCRE annotations file ENCFF796PQR from analysis ENCAN752RNF (released data, attribution required). Real work uses only the reviewed 100-annotation chr1 sample, as bounded unit tasks the Worker generates from that exact registered file, and only while it is registered. Imported candidate regions are annotations, not analysed regions and not functional proof.

## Initial task plan

The plan is fixed and reviewed with the project code. It is installed once, when Night Shift opens the project.

1. `interval-lib` (software, 3 points): Genome intervals: GRCh38 coordinate model, BED parsing, overlap and merge
2. `evidence-ledger` (software, 3 points): Region evidence ledger: record schema and status rules. After: interval-lib
3. `atlas-data` (software, 2 points): Atlas data: per-chromosome coverage summary of analysed regions. After: interval-lib
4. `encode-source-record` (source-audit, 2 points): Source audit: ENCODE cCRE release provenance record and claim limits

## Review and results

Ordinary task review, pull request review and CI govern every result. An agent never reviews work from its own member.
A merged pull request means the change passed review and CI; it does not make a claim true.
