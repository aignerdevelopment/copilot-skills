# copilot-skills — pinned source for harnessator

A governed **[harnessator](https://github.com/aignerdevelopment/harnessator)
source**, produced by `harnessator harvest` from
[github/awesome-copilot](https://github.com/github/awesome-copilot) at
commit `5269f7e` — **448 skills, MIT licensed** (the upstream `LICENSE`
travels with them), content byte-identical to upstream `skills/`.
The manifest is a schema-2 **pointer** (source format v1.1): registration is
live via `[discover]`, so it cannot drift - the pinned ref and commit are
recorded in `UPSTREAM.md`, refreshed by the harnessator 'Bridge refresh' workflow.

Scope honesty: only the skills collection is bridged. The repo's
`.instructions.md` / `.prompt.md` copilot-dialect files wait for
harnessator's copilot expansion adapter, and `docs/`/`cookbook/` are
not agent components. See `HARVEST-NOTES.md` for the reviewed sanitize
findings (all documentation examples and one deliberate decoy).

## Consume it

```sh
harnessator source add https://github.com/aignerdevelopment/copilot-skills.git --ref v0.2.0
harnessator enable copilot-skills:quality-security   # a stack profile - see below
harnessator setup
```

**Prefer a profile over `:default`.** 448 skills is a directory, not a
daily toolchain — each enabled skill adds its description to your
agent's discovery index. The curated profiles are the recommended
entry; `harnessator search <topic>` (after adding the source) is the
right way to cherry-pick individual skills from the rest.

| profile | theme |
|---|---|
| `quality-security` | review, testing, security, compliance, triage |
| `agent-dev` | agents, prompts, MCP, orchestration, evals |
| `azure-dotnet` | Azure, dotnet, Aspire, readiness |
| `python-stack` | python, django, flask, pandas, pytest |
| `web-frontend` | react, next, tailwind, vite, UI |
| `default` | every upstream skill, live (wildcard) - deliberately heavy, use with intent |

## Update policy

Same as the other bridges: re-harvest from an upstream commit, keep
the profile membership honest (keyword picks reviewed against the real
id list), refresh this README's commit line, one reviewable commit per
upstream refresh, tag `v0.N.0`. Consumers move by lockfile update, not
surprise. Attribution: skills are authored by GitHub's community and
the awesome-copilot maintainers — this is a pinned mirror for
governed consumption, not a fork.
