# Harvest notes - copilot-skills bridge

Harvested 2026-10-30 from https://github.com/github/awesome-copilot
(commit 5269f7e, skills/ collection only - 448 components, MIT,
LICENSE carried). The repository's .instructions.md/.prompt.md
copilot-dialect files and docs/cookbook content are NOT part of this
bridge: they await harnessator's copilot expansion adapter.

## Sanitize findings - reviewed before publishing

All findings below are documentation examples or deliberate decoys,
reviewed line-by-line: amqp://guest:guest@localhost and
Password=... connection-string samples (Aspire docs), C:/home user
paths in batch/cygwin/RFC-8805 reference material, and the
sk-abc123... "api-key" inside mcp-security-audit's own bad-config
example (that skill teaches detection of exactly this). No real
credentials present.

  credentials-in-url at aspire/references/architecture.md:124 ://guest…est@ (skill/aspire)
  secret-assignment at aspire/references/architecture.md:322 apiKey =…eter (skill/aspire)
  personal-path at batch-files/references/batch-files-and-functions.md:75 C:\U*** (skill/batch-files)
  personal-path at batch-files/references/cygwin.md:87 C:\U*** (skill/batch-files)
  personal-path at batch-files/references/cygwin.md:90 /hom*** (skill/batch-files)
  secret-assignment at cypress-flake-fixer/references/removed-apis.md:39 apiKey: …_KEY (skill/cypress-flake-fixer)
  credentials-in-url at data-breach-blast-radius/references/hardening-playbook.md:153 ://u*** (skill/data-breach-blast-radius)
  secret-assignment at dotnet-mcp-builder/references/transport-stdio.md:90 apiKey =…able (skill/dotnet-mcp-builder)
  personal-path at geofeed-tuner/references/rfc8805.txt:567 /home/st…rds/ (skill/geofeed-tuner)
  personal-path at geofeed-tuner/references/rfc8805.txt:572 /home/st…rds/ (skill/geofeed-tuner)
  credentials-in-url at mcp-security-audit/SKILL.md:104 ://admin…123@ (skill/mcp-security-audit)
  secret-assignment at namecheap/namecheap.py:168 api_key …ials (skill/namecheap)
  personal-path at noob-mode/references/examples.md:11 /Use*** (skill/noob-mode)
  personal-path at noob-mode/references/examples.md:38 /Use*** (skill/noob-mode)
  secret-assignment at phoenix-tracing/references/sessions-typescript.md:26 apiKey: …_KEY (skill/phoenix-tracing)
  secret-assignment at phoenix-tracing/references/setup-typescript.md:33 apiKey: …_KEY (skill/phoenix-tracing)
  secret-assignment at pinecone-rag/SKILL.md:50 api_key=…_KEY (skill/pinecone-rag)
  secret-assignment at react18-string-refs/references/patterns.md:67 password…alue (skill/react18-string-refs)
  secret-assignment at react18-string-refs/references/patterns.md:92 password…alue (skill/react18-string-refs)
  personal-path at rhino3d-scripts/references/macros-and-loading.md:34 C:\U*** (skill/rhino3d-scripts)
  personal-path at sandbox-npm-install/SKILL.md:63 /hom*** (skill/sandbox-npm-install)
  personal-path at sandbox-npm-install/SKILL.md:80 /hom*** (skill/sandbox-npm-install)
  personal-path at sandbox-npm-install/scripts/install.sh:13 /hom*** (skill/sandbox-npm-install)
  secret-assignment at security-review/references/secret-patterns.md:142 API_KEY:…here (skill/security-review)
  secret-assignment at security-review/references/secret-patterns.md:160 password…word (skill/security-review)
  private-key at security-review/references/vuln-categories.md:174 -----BEG…---- (skill/security-review)
