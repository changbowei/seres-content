# Working with SERES content

This repository is intended to be checked out at `content/` inside the SERES
repository. The schema, validators, CLI, and simulation engine are maintained
in the parent SERES repository.

Before changing KB data, read the parent repository's `AGENTS.md` and the
schema and knowledge-acquisition documents it requires. Run validation from
the parent checkout, where the default KB path is `content/kb`.

Simulation snapshots and event logs are generated files. They are ignored for
new runs and should be force-added only when intentionally publishing a
simulation. A published simulation should include its `provenance.json`.

Commit KB and published simulation changes here first. Then commit the updated
`content/` submodule pointer in the parent SERES repository.
