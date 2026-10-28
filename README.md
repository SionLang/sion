# Sion

A programming language designed for AI agents: few tokens, memory safe, no null, effect-tracked, with machine-readable diagnostics.

**Status:** M0 (specification + bootstrap seed). Nothing here compiles yet.

## Plan
1. `sion-seed` (throwaway, Rust) compiles Sion-0 to x86-64 (PE/ELF) and WASM.
2. The compiler is rewritten in Sion-0 and compiled by the seed.
3. The compiler compiles itself until output is byte-identical (fixed point).
4. The seed is archived; this repo becomes pure Sion.

## Repos
| Repo | Purpose |
|---|---|
| sion | Compiler and CLI (`sion check/run/test/ship`) |
| sion-spec | Formal specification |
| sion-seed | Bootstrap compiler (temporary) |
| sion-tests | Conformance tests shared by every compiler stage |

File extension: `.sn`
