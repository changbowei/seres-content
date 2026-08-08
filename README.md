# SERES Content

This repository contains knowledge and published simulation data used by
[SERES](https://github.com/aniemerg/seres).

## Content Line

This repository is `changbowei`'s independently maintained content line.
Results from it should identify both the SERES commit and this repository's
content commit; they should not be treated as data from another contributor's
content line.

It is normally checked out as the `content/` submodule inside a SERES checkout:

```text
seres/
  content/
    kb/
    simulations/
```

The parent SERES commit pins an exact commit of this repository. Clone SERES
with its content by running:

```bash
git clone --recurse-submodules git@github.com:aniemerg/seres.git
```

`kb/` is the curated knowledge base. `simulations/` contains simulation runs
that have been deliberately published. New simulation output is ignored by
default; use `git add -f` when a run should become part of the published
content.

The canonical schema and simulation engine live in SERES. Compatibility is
identified by the pair of commit hashes recorded by the SERES checkout and by
each simulation's `provenance.json`.
