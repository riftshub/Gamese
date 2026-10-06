# Gamese

Monorepo combining two N64 game projects, each kept in its own directory with its full upstream history:

| Directory | Upstream | Description |
|---|---|---|
| [`sm64/`](sm64/) | [n64decomp/sm64](https://github.com/n64decomp/sm64) | Super Mario 64 decompilation |
| [`DNZHRecomp/`](DNZHRecomp/) | [sonicdcer/DNZHRecomp](https://github.com/sonicdcer/DNZHRecomp) | Duke Nukem: Zero Hour static recompilation |

Each project builds independently; see the README/BUILDING docs inside each directory. Neither project ships game assets: you must supply your own legally-obtained ROMs.

DNZHRecomp depends on submodules (declared in the root `.gitmodules`). Fetch them with:

```sh
git submodule update --init --recursive
```
