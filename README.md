# DocBot

**Documentation that keeps up with your code.**

## The problem

Every codebase ends up with a documentation folder nobody trusts. Last updated three years ago, written by someone who left, contradicted by the actual code. Manual documentation loses to delivery pressure every time.

## How DocBot works

Install DocBot on a repository. When a PR is opened, DocBot reads the diff, generates documentation for the changed files, and commits it to a `_docs/` folder in your repo. Your PR review shows code changes and doc changes side by side. Merging the PR ships both.

Three layers of output: per-file READMEs, directory summaries, and a master index. Architecture diagrams via Mermaid. Dependency catalogues with licence data for compliance audits.

Free tier: 250,000 lifetime tokens plus access to a shared 250M monthly pool. No credit card.

---

## Key features

- **Three-layer documentation structure** — per-file READMEs, directory summaries, and a master index that stays navigable as the codebase grows
- **Architecture diagrams** — Mermaid diagrams generated from your code (system architecture, workflows, data models, component dependencies, API integrations); GitHub renders them natively in your repo
- **Dependency catalogue** — every package from `package.json`, `requirements.txt`, `Cargo.toml` and others, with licence data fetched from npm, PyPI, and crates.io. Generated as `DEPENDENCIES.md` for compliance audits and SBOMs
- **Runs on GPT-5-nano** — roughly 70–90% cheaper than the GPT-4 / Claude-class models most AI docs tools default to. Documentation is a structure-and-accuracy task, not a creative-writing one, and nano holds up well for it
- **Multi-language support** — Python, JavaScript, TypeScript, Java, C#, Go, Rust, PHP, and more
- **PR-based automation** — documents changed files automatically on every pull request, with `[skip ci]` commits so it doesn't loop
- **Flexible configuration** — branch filtering, manual approval workflows, custom exclusions via `.github/wai-docbot.yml`
- **Full repository rebuilds** — regenerate all documentation via the `wai-docs-update` branch
- **Manual re-runs** — comment `/docbot-rerun` to regenerate docs after PR updates

## Pricing

| Tier | Price | Tokens / month | Status |
|------|-------|----------------|--------|
| **Free** | **$0** | 250K lifetime + shared 250M pool | ✅ Live |
| Entry | $10/mo | 250K | Launching soon |
| Small | $50/mo | 1.5M | Launching soon |
| Medium | $150/mo | 5M | Launching soon |
| Enterprise | $500+/mo | 20M+ | Launching soon |

No per-seat fees on any tier. Add unlimited team members. Pay only for tokens used.

Free tier covers roughly 40–50 files of documentation lifetime, plus access to a shared 250M monthly pool for ongoing PR documentation. Small repositories run comfortably on free forever.

## Setup

### Quick installation (3 minutes)

1. **[Install AI Document Creator on GitHub Marketplace](https://github.com/apps/ai-document-creator)** — one click, no credit card
2. *(Optional)* Add `.github/wai-docbot.yml` to configure docs folder path, branch filters, and file exclusions
3. Open a pull request — DocBot generates documentation in the `_docs/` folder
4. Review and merge

### Configuration

Create `.github/wai-docbot.yml` to customise DocBot's behaviour:

- **Cost control** — exclude build artifacts, dependencies, and generated files to manage token usage
- **Branch filtering** — control which target branches trigger documentation (supports wildcards)
- **Manual approval** — require explicit approval before generating docs on each PR
- **File selection** — specify which file extensions to document and which paths to exclude
- **Documentation preferences** — include code links, examples, and control root file documentation
- **Overage management** — enable or turn off billing for usage beyond tier limits

For the complete configuration reference, examples, and best practices, see the [setup guide](https://woden-ai.com/setup/docbot).

## How it works

### Documentation generation

DocBot generates three layers of documentation:

1. **File-level READMEs** — each source file gets documentation explaining purpose, functions, dependencies, and usage patterns
2. **Directory-level READMEs** — each folder receives an overview of its purpose, contained modules, and architecture
3. **Master index** — top-level README with complete repository map and navigation

### Workflow

1. **Automatic PR processing** — open a pull request, and documentation is generated automatically for changed files
2. **Token tracking** — each PR comment shows token usage and remaining allocation
3. **Commit to repository** — documentation commits to the `_docs/` folder with `[skip ci]` tag
4. **Manual re-runs** — comment `/docbot-rerun` to regenerate after PR updates
5. **Full rebuilds** — create the `wai-docs-update` branch to regenerate all repository documentation

## Privacy and data residency

- Processed in **Azure UK South**. GDPR compliant.
- Code is processed in-request and **never stored** beyond the request lifecycle.
- **No training on customer code** — covered contractually by Microsoft's Azure OpenAI Data Protection Addendum.
- All traffic encrypted in transit. Webhook signatures validated. App private key held in Azure Key Vault.
- Minimal GitHub permissions (Contents R/W, PRs R/W).
- Detailed audit log of every operation visible in the Admin Portal at [woden-ai.com/portal](https://woden-ai.com/portal).

## Support

- Full setup guide: [woden-ai.com/setup/docbot](https://woden-ai.com/setup/docbot)
- Priority support via GitHub issues or auto-generated emails for paid customers (48-hour SLA): [GitHub Issues](https://github.com/wodenagi/docbot/issues)
- **Reporting bugs**: [GitHub Issues](https://github.com/wodenagi/docbot/issues)
- **Announcements & feature requests**: [GitHub Discussions](https://github.com/orgs/wodenagi/discussions)

---

**Get started**: [Install on GitHub Marketplace](https://github.com/apps/ai-document-creator)

---

Built by [Woden AI](https://woden-ai.com) · [Product page](https://woden-ai.com/products/docbot) · [Setup guide](https://woden-ai.com/setup/docbot)
