# AI Document Creator - Automated Documentation Generation

## The Problem

Development teams struggle to maintain comprehensive, up-to-date documentation. Manual documentation takes a lot of time, quickly becomes outdated, and is often deprioritized under delivery pressure. This results in technical debt, slows onboarding, and makes code reviews more challenging for both developers and product managers overseeing deliverables.

## The Solution

AI Document Creator automatically produces comprehensive documentation for your entire repository and every subsequent pull request. Your documentation remains synchronized with your code without manual effort, ensuring that developers always have current references and that product managers can verify deliverables against the latest documentation.

**Start free with 250,000 tokens** - enough to document 40-50 files or multiple PRs with full product access.

---

## Key Features

- **Three-Level Documentation Structure**: Per-file READMEs, directory summaries, and master repository index
- **AI-Powered Analysis**: Context-aware documentation that understands code structure, functions, and relationships
- **Multi-Language Support**: Python, JavaScript, TypeScript, Java, C#, Go, Rust, PHP, and more
- **PR-Based Automation**: Documents changed files automatically on every pull request
- **Flexible Configuration**: Branch filtering, manual approval workflows, custom exclusions via `.github/wai-docbot.yml`
- **Full Repository Rebuilds**: Regenerate all documentation via `wai-docs-update` branch
- **Cost-Effective**: 70-90% cheaper than premium AI models, optimized specifically for documentation tasks
- **Manual Re-runs**: Use `/docbot-rerun` comment to regenerate docs after PR updates

## Pricing

| Tier | Price | Tokens | Availability | Approx. Files/Month |
|------|-------|--------|--------------|---------------------|
| **Free** | **Free** | **250K lifetime** + 250M monthly pool (shared) | **✅ Available Now** | ~40-50 total |
| **Entry** | $10/mo | 250K/mo | Coming Soon | ~60-75 |
| **Small** | $50/mo | 1.5M/mo | Coming Soon | ~360-450 |
| **Medium** | $150/mo | 5M/mo | Coming Soon | ~1,200-1,500 |
| **Enterprise** | $500/mo | 20M+/mo | Coming Soon | ~4,800-6,000+ |

**Free tier includes** full product access with all features, all programming languages, custom configuration, and community support.

**Paid tiers** (pending GitHub verification) include unlimited monthly allocations, priority support with 48-hour SLA, and advanced features.

## Setup

### Quick Installation (3 minutes)

1. **[Install AI Document Creator](https://github.com/apps/ai-document-creator)** on your repository
2. Open a pull request
3. Documentation is generated automatically in the `wai_docs/` folder
4. Review and merge

### Configuration (Recommended)

Create `.github/wai-docbot.yml` to customize AI Document Creator's behaviour:

**Configuration benefits:**
- **Cost Control**: Exclude build artifacts, dependencies, and generated files to manage token usage
- **Branch Filtering**: Control which target branches trigger documentation (supports wildcards)
- **Manual Approval**: Require explicit approval before generating docs on each PR
- **File Selection**: Specify which file extensions to document and which paths to exclude
- **Documentation Preferences**: Include code links, examples, and control root file documentation
- **Overage Management**: Enable or turn off billing for usage beyond tier limits

**For complete configuration reference, examples, and best practices**, visit the [setup guide](https://woden-ai.com/setup/docbot).

## How It Works

### Documentation Generation

AI Document Creator generates three levels of documentation:

1. **File-Level READMEs**: Each source file gets documentation explaining purpose, functions, dependencies, and usage patterns
2. **Directory-Level READMEs**: Each folder receives an overview of its purpose, contained modules, and architecture
3. **Master Index**: Top-level README with complete repository map and navigation

### Workflow

1. **Automatic PR Processing**: Open a pull request, and documentation is generated automatically for changed files
2. **Token Tracking**: Each PR comment shows token usage and remaining allocation
3. **Commit to Repository**: Documentation commits to `wai_docs/` folder with `[skip ci]` tag
4. **Manual Re-runs**: Comment `/docbot-rerun` to regenerate after PR updates
5. **Full Rebuilds**: Create `wai-docs-update` branch to regenerate all repository documentation

### Privacy & Security

- Code processed in real-time, never stored
- Encrypted API connections
- Minimal GitHub permissions (Contents R/W, PRs R/W)
- Per-account token tracking
- Full audit logging

## Support

- Full guide available at: [woden-ai.com/setup/docbot](https://woden-ai.com/setup/docbot)
- Priority support via GitHub issues or auto-generated emails for paid customers (48-hour SLA): [GitHub Issues](https://github.com/wodenagi/docbot/issues)
- **Reporting Bugs**: [GitHub Issues](https://github.com/wodenagi/docbot/issues)
- **Announcements & Feature Requests**: [GitHub Discussions](https://github.com/orgs/wodenagi/discussions)

---

**Get Started**: [Install AI Document Creator](https://github.com/apps/ai-document-creator)

---

Built by Woden AI · [Website](https://woden-ai.com) · [Pricing](https://woden-ai.com/products)
