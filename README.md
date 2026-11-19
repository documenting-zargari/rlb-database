# RLB Database

Periodic backup of the evolving RLB Database, preserving legacy data.

The data has been sanitized regarding personal information in conformance with EU law.

This repository contains

- A MySQL dump from the early 2000s, the basis of this data collection
- An ArangoDB repository that represents this data, as well as later corrections and additions.

## Current database dumps

A scheduled workflow (`.github/workflows/publish-dump.yml`) dumps the live database every day
and publishes a [release](https://github.com/documenting-zargari/rlb-database/releases) whenever
the data has changed. Each release lists the document count per collection.

Newest dump (stable URL):

    https://github.com/documenting-zargari/rlb-database/releases/latest/download/rld-arangodump.tar.gz

To run your own copy of the RLD from it, see
[drd-django/deploy/RESTORE.md](https://github.com/documenting-zargari/drd-django/blob/dev/deploy/RESTORE.md).

The `arango/` folder in this repository is an older snapshot (20 July 2026); use the releases instead.
