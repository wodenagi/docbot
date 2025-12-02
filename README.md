# AI Document Creator - Automated Documentation Generation

## Transform Code Into Documentation, Automatically

AI Document Creator uses advanced AI (appropriate language models) to automatically generate comprehensive documentation for your code changes, ensuring your docs stay up-to-date with every pull request.

## 🚀 Start FREE with 150,000 Tokens!

**Document your entire moderate-sized repository or process dozens of PRs** - completely free! Get full access to all features with our generous free tier. Perfect for exploring the product and understanding the value before committing to a paid plan.

**✨ What you get for free:**
- 150,000 tokens (enough to document 25-30 code files)
- Full product access - no feature restrictions
- All programming languages supported
- Custom configuration via `.github/wai-docbot.yml`
- Branch filtering and approval workflows
- Comprehensive documentation generation

**📊 Fair Usage:** Free tier usage is subject to a fair monthly usage allocation (250M tokens shared across all free tier users) to ensure sustainable service for everyone. This ensures the service remains available and responsive for all users while we grow toward verification and paid tier launch.

**💡 Coming Soon:** More powerful paid tiers for high-volume usage and enterprise features - currently building toward GitHub verification (100 installations required).

---

## ✨ Key Features

### 🤖 AI-Powered Generation
- **Intelligent Analysis**: appropriate language models analyzes your code changes and generates clear, accurate documentation
- **Context-Aware**: Understands code structure, functions, classes, and their relationships
- **Professional Quality**: Human-readable documentation that explains what the code does and why
- **Multiple Languages**: Supports Python, JavaScript, TypeScript, Java, C#, Go, and more

### 📚 Automatic Documentation
- **Per-File README**: Creates individual README.md for each code file explaining its purpose and functionality
- **Directory Summaries**: Generates README.md for each directory showing overview of contained modules
- **Master Index**: Creates top-level README.md with complete repository documentation map
- **PR-Based Updates**: Generate docs automatically when PRs are opened or updated
- **Incremental Generation**: Only documents changed files for efficiency
- **Full Repository Rebuilds**: Option to regenerate all documentation at once
- **Custom Folder Structure**: Configure where docs are stored (default: `wai_docs/`)
- **⚠️ File Exclusions Critical**: Properly exclude build artifacts, dependencies, and generated files to maintain documentation readability and control costs
- **Incremental Rebuilds**: Full repository documentation via `wai-docs-update` branch or `[DOCS-REBUILD]` tag

### 💰 Cost-Effective AI
- **70-90% Cheaper**: Uses appropriate language models instead of expensive Highend AI Models (GPT5/Claude etc.)
- **Right Tool, Right Job**: Optimized for documentation generation tasks
- **Token-Based Pricing**: Only pay for what you need (coming soon)
- **Free Tier**: Start with 150,000 tokens - document a moderate repo or dozens of PRs!

### ⚙️ Flexible Configuration
- **Branch Filtering**: Control which target branches trigger documentation (supports wildcards like `release/*`)
- **Manual Approval Mode**: Require explicit approval before generating docs on each PR (`require_pr_approval: true`)
- **Exclude Patterns**: Ignore build artifacts, dependencies, and generated files
- **Custom Docs Folder**: Choose where documentation is stored
- **Free Tier**: 100K total tokens to get started - full product access!
- **🔮 Coming Soon**: Paid plans from $10/mo (250K tokens) to $500/mo (20M+ tokens)
- **🔮 Coming Soon**: Release documentation generator with custom tone configuration

## 🚀 Perfect For

- **Trying Before Buying**: 150K free tokens let you experience the full product
- **Small to Medium Projects**: Document entire repos with the generous free allocation
- **Active Development Teams**: Keep documentation current without manual effort (free tier great for moderate activity)
- **Open Source Projects**: Maintain contributor-friendly documentation automatically
- **API Development**: Generate clear API documentation from code
- **Onboarding**: Help new developers understand codebases faster
- **Compliance**: Maintain documentation standards across projects

## 📈 Benefits

- **Always Up-to-Date**: Docs generated with every code change
- **Save Developer Time**: No more manual documentation writing
- **Consistent Quality**: AI ensures uniform documentation standards
- **Reduce Technical Debt**: Never let documentation fall behind again
- **Better Code Reviews**: Reviewers see documentation alongside code changes
- **Faster Onboarding**: New team members have comprehensive docs available

## 💡 How It Works

### 🏗️ Documentation Structure
AI Document Creator generates **three levels of documentation**:

1. **File-Level READMEs**: Each source file gets its own README.md explaining:
   - Purpose and functionality
   - Key classes, functions, and exports
   - Dependencies and relationships
   - Usage patterns and examples

2. **Directory-Level READMEs**: Each folder gets a README.md with:
   - Overview of the directory's purpose
   - List of contained modules
   - Architecture and organization notes
   - Common patterns used

3. **Master Index**: Top-level README.md providing:
   - Complete repository documentation map
   - High-level architecture overview
   - Navigation to all documented modules
   - Quick reference guide

**⚠️ Important**: With hundreds of files documented, **proper file exclusions are essential** to:
- Keep documentation focused and readable
- Avoid documenting build artifacts, dependencies, or generated code
- Control token usage and costs
- Maintain meaningful documentation hierarchy

### 1️⃣ Install & Configure
- [Install AI Document Creator](https://github.com/apps/wagi-docbot) on your repository
- **Configure exclusions** in `.github/wai-docbot.yml` (recommended for optimal performance)
- Start with **150K free tokens** - document your entire moderate repo or dozens of PRs!

### 2️⃣ Automatic Processing
- Open a PR and documentation generates automatically
- AI analyzes changed files and creates comprehensive docs
- Documentation committed to `wai_docs/` folder in your repository (with `[skip ci]` to avoid triggering CI/CD pipelines)
- **Free tier**: Process PRs until you reach 150K tokens - plenty for most moderate projects!

### 3️⃣ Grow with Us
- Free tier: **100K tokens** - experience the full product!
- Configure branch filtering, approval workflows, and exclusions
- Track your usage via GitHub comments on each PR
- **Coming soon**: Paid tiers from $10/mo (250K tokens) to $500/mo (20M+ tokens) - currently working toward GitHub verification

### 💡 Manual Re-runs
Need to regenerate docs after making quick changes to your PR? Simply comment:
```
/docbot rerun
```

**What it does:**
- Immediately regenerates documentation for the current PR
- Bypasses the 5-minute duplicate check (safety feature that prevents accidental re-runs)
- Re-analyzes all changed files with latest code
- Available for both free and paid tiers (counts against your token allocation)

**Perfect for:**
- Made quick fixes after initial documentation
- Updated function signatures or parameters
- Want to see how config changes affect output
- Need fresh docs without closing/reopening the PR

### 4️⃣ Full Repository Rebuilds
- Create branch `wai-docs-update` from your main branch
- Create an empty commit: `git commit --allow-empty -m "Trigger full documentation rebuild"`
- Push and create PR to trigger full repo scan
- DocBot posts token estimate and cost
- Comment `/docbot rebuild approve` to proceed
- Complete documentation with master index generated

**Alternative triggers:**
- Include `[DOCS-REBUILD]` in PR title from any branch
- Use branch name containing `wai-docs-update`

## 📊 Pricing Tiers

| Tier | Price | Tokens | Availability | Approx. Files/Month |
|------|-------|--------|--------------|---------------------|
| **Free** | **Free** | **150K lifetime** + 250M monthly pool (shared) | **✅ Available Now** | ~25-30 total |
| **Entry** | $10/mo | 250K/mo | 🔮 Coming Soon | ~60-75 |
| **Small** | $50/mo | 1.5M/mo | 🔮 Coming Soon | ~360-450 |
| **Medium** | $150/mo | 5M/mo | 🔮 Coming Soon | ~1,200-1,500 |
| **Enterprise** | $500/mo | 20M+/mo | 🔮 Coming Soon | ~4,800-6,000+ |

**Free tier includes:**
- ✅ 150,000 lifetime tokens - document entire repos or dozens of PRs
- ✅ 250M monthly shared pool across all free tier users for fair usage
- ✅ All programming languages supported
- ✅ Full product features - no restrictions
- ✅ Custom configuration via `.github/wai-docbot.yml`
- ✅ Branch filtering and approval workflows
- ✅ Community support and documentation
- 📊 Subject to fair monthly usage allocation (250M tokens shared across all free users)

**Paid tiers coming soon** (pending GitHub verification - need 100 installations):
- Unlimited monthly token allocations
- Priority email support (24-hour SLA)
- Advanced features and integrations
- Dedicated account management (Enterprise)

## 🔧 Configuration Example

### ⚠️ Configuration is Critical for Optimal Performance

While AI Document Creator works with default settings, **proper YAML configuration is essential** for:
- **Cost Control**: Exclude build artifacts, dependencies, and generated files to avoid wasting tokens
- **Quality Documentation**: Filter out test files, minified code, and non-source files
- **Branch Control**: Specify which branches trigger documentation
- **Folder Organization**: Choose where docs are stored

**Recommended:** Always create `.github/wai-docbot.yml` in your repository with proper exclusions for your project type.

Create `.github/wai-docbot.yml` in your repository:

```yaml
# Documentation folder (default: wai_docs)
docs_folder: "wai_docs"

# Allowed target branches for PR documentation (default: main, master, develop, release/*, wai-docs-update)
allowed_base_branches:
  - main
  - master
  - develop
  - release/*  # Matches release/1.0.0, release/v2.0, etc.
  - hotfix/*   # Matches hotfix/critical-bug, hotfix/security-patch, etc.
  - staging
  - wai-docs-update  # For full rebuilds

# Overage billing - MUST be explicitly enabled to allow charges beyond tier limits
# When enabled:
#   - You'll be asked to approve overages via PR comment reactions
#   - GitHub automatically charges your payment method for approved overages
#   - Charges appear on your GitHub Marketplace bill
# When disabled (default):
#   - PRs that exceed your tier limit will be blocked
#   - You'll see a message with instructions to enable overages
overage_enabled: false  # Set to true to enable automatic overage billing

# Documentation preferences
preferences:
  # Include links to source code line numbers in GitHub
  include_code_links: true
  
  # Include usage examples in function documentation
  include_examples: true

  # Require manual approval before generating documentation
  # When true, you must comment "/docbot approve" on each PR to generate docs
  # When false, documentation is generated automatically (default)
  require_pr_approval: true
  
  # Document root-level files (e.g., setup.py, main.py in repository root)
  # Creates a separate README for root files alongside the master index
  document_root_files: true

# Code file extensions to document (INCLUSION LIST)
# Only files with these extensions will be processed
# This provides explicit control and prevents accidental processing of data files
include_extensions:
  # Python
  - ".py"
  
  # JavaScript/TypeScript
  - ".js"
  - ".jsx"
  - ".ts"
  - ".tsx"
  - ".mjs"
  - ".cjs"
  
  # Web
  - ".html"
  - ".css"
  - ".scss"
  - ".sass"
  - ".less"
  
  # C/C++
  - ".c"
  - ".cpp"
  - ".cc"
  - ".cxx"
  - ".h"
  - ".hpp"
  - ".hxx"
  
  # C#/.NET
  - ".cs"
  - ".vb"
  - ".fs"
  
  # Java/Kotlin
  - ".java"
  - ".kt"
  - ".kts"
  
  # Go
  - ".go"
  
  # Rust
  - ".rs"
  
  # Ruby
  - ".rb"
  
  # PHP
  - ".php"
  
  # Swift
  - ".swift"
  
  # Shell scripts
  - ".sh"
  - ".bash"
  - ".zsh"
  - ".fish"
  
  # PowerShell
  - ".ps1"
  - ".psm1"
  - ".psd1"
  
  # SQL
  - ".sql"
  
  # R
  - ".r"
  - ".R"
  - ".scala"
  - ".dart"
  - ".lua"

  # Go
  - ".go"

  # Infrastructure as Code
  - ".tf"    # Terraform
  - ".yaml"  # YAML (for Kubernetes, etc.)
  - ".yml"   # YAML (for Kubernetes, etc.)
  - ".bicep" # Bicep

# Files and patterns to exclude (EXCLUSION LIST)
# Applied AFTER extension filtering - use for specific paths/directories
exclude:
  # Custom exclusions for this project
  # - "iac/**" # example to exclude your Infrastructure code
  
  # Dependencies and package managers
  - "node_modules/**"
  - "vendor/**"
  - "**/package-lock.json"
  - "**/__pycache__/**"
  
  # Build outputs
  - "dist/**"
  - "build/**"
  - "**/build/**"
  - "**/bin/**"
  - "**/obj/**"
  - "**/target/**"
  - "**/.next/**"
  - "**/coverage/**"
  
  # Minified/bundled files
  - "**/*.min.js"
  - "**/*.bundle.js"
  - "**/*.map"
  
  # IDE and version control
  - ".git/**"
  - ".gitignore"
  - "**/.gitignore"
  - "**/.vscode/**"
  - "**/.idea/**"
  - "**/.pytest_cache/**"
  
  # Environment and secrets
  - "**/.env*"
  - "**/local.settings.json"
  - "**/credential.json"
  - "**/*.pem"
  - "**/*.key"
  - "**/secrets/**"
  
  # Existing documentation (prevents circular documentation)
  - "**/*.md"
  - "docs/**"
  - "wai_docs/**"
  
  # Logs and temporary files
  - "**/*.log"
  - "**/tmp/**"
  - "**/*.tmp"
```

**Note**: The default configuration uses a **hybrid inclusion/exclusion approach**:
1. **Inclusion list** (`include_extensions`) specifies which code file types to document (e.g., `.py`, `.js`, `.ts`)
2. **Exclusion list** (`exclude`) filters out specific paths (e.g., `node_modules/`, `build/`)

This ensures only actual code files are documented, preventing accidental processing of data files, configs, or build artifacts.

## 📝 Example Output

```markdown
# API Handler Documentation

## Overview
This module provides HTTP request handling for the user authentication API endpoints.

## Functions

### authenticate_user(username: str, password: str) -> dict
Validates user credentials and generates authentication token.

**Parameters:**
- `username` (str): User's login identifier
- `password` (str): User's password (hashed)

**Returns:**
- dict: Authentication response with token and user info

**Raises:**
- `AuthenticationError`: When credentials are invalid
- `DatabaseError`: When user lookup fails
```

## 🔒 Privacy & Security

- **Code Never Stored**: Your code is only processed, never saved
- **Secure API Calls**: All AI processing uses encrypted connections
- **GitHub Permissions**: Minimal required permissions (Contents R/W, PRs R/W)
- **Token Security**: Billing tokens tracked per account, never shared
- **Audit Logging**: Full operation history for transparency

## 🎁 Free Tier

Every account starts with **150,000 lifetime tokens** to explore the full product! That's enough to document:
- **~25-30 code files** with comprehensive documentation
- Multiple PRs across different repositories
- Full repository rebuilds for small-medium projects

**No subscription required.** Install, start documenting, and upgrade when you need more tokens!

## 🚦 Getting Started

### Quick Start (3 minutes)
1. [Install AI Document Creator](https://github.com/apps/wagi-docbot)
2. Open a PR in your repository
3. Documentation generates automatically (with `[skip ci]` tags to avoid triggering CI/CD)
4. Review the comprehensive docs in `wai_docs/` folder
5. Upgrade to a paid plan when you reach the free tier limit

### Full Setup Guide
Visit our [setup guide](https://woden-ai.com/setup/docbot) for detailed configuration instructions.

## 💬 Support & Community

### 🔧 Automatic Error Reporting
When issues occur, AI Document Creator automatically generates a **pre-filled support email** with:
- Error details and context
- Repository and PR information
- Configuration snapshot
- Relevant logs

**Simply click the mailto link in the error message** to send the report directly to our support team. No need to manually gather diagnostics!

### Contact & Resources
- **Setup Issues**: [Configuration Guide](https://woden-ai.com/setup/docbot)
- **Bug Reports & Issues**: [GitHub Repository](https://github.com/wodenagi/docbot)
- **Feature Requests**: [GitHub Discussions](https://github.com/wodenagi/docbot/discussions)
- **Community Support**: Join discussions and share feedback on our [GitHub repository](https://github.com/wodenagi/docbot)
- **Billing Questions**: support@woden-ai.com
- **Technical Support**: Included with all paid tiers - 24-hour response guarantee

## 🌟 Why AI Document Creator?

### The Problem
- Manual documentation is time-consuming
- Docs quickly become outdated
- Inconsistent documentation quality
- Documentation often skipped under pressure

### Our Solution
- **Automatic**: Documentation generated on every PR
- **AI-Powered**: Intelligent, context-aware content
- **Cost-Effective**: 70-90% cheaper than Highend AI Models (GPT5/Claude etc.)
- **Free to Start**: 150K lifetime tokens to explore the full product
- **Flexible**: Works with your workflow and standards

### The Result
- ✅ Always current documentation
- ✅ Saved developer hours
- ✅ Better code comprehension
- ✅ Faster onboarding
- ✅ Reduced technical debt

## 🔮 Coming Soon

### ✨ Custom Documentation Prompts

Customize the AI's documentation style to match your team's preferences:

- **Custom Tone & Voice**: Configure AI prompts to match your documentation style and terminology
- **Language Preferences**: Control verbosity, technical depth, and explanation style
- **Brand Alignment**: Ensure generated docs use your organization's preferred language patterns
- **Per-Repository Config**: Set different documentation styles for different projects
- **Template Snippets**: Define custom templates for common documentation patterns

Perfect for:
- Teams with specific documentation standards
- Organizations with branded communication requirements
- Projects requiring different documentation depths
- Multi-language or multi-audience documentation

*Empower your team to generate docs that sound exactly how you want them!*

### 📦 Release Documentation Generator
Automate customer-facing release notes for GitHub Releases:

- **Automatic Release Notes**: Generate professional release documentation from GitHub Release tags
- **Custom Tone & Voice**: Add custom prompt snippets to match your brand's communication style
- **Customer-Focused**: AI transforms technical changes into customer-friendly benefits
- **Separate Storage**: Release docs stored in dedicated folder (e.g., `releases/`)
- **Version History**: Maintain complete release documentation history

Perfect for:
- Customer-facing product updates
- SaaS changelog generation
- Open source release announcements
- Professional release communications

*Stay tuned for this exciting feature!*

### 🔄 Full Repository Rebuild (Complete Regeneration)

Enhanced rebuild workflow for complete documentation regeneration:

- **Complete Regeneration**: Delete and rebuild all documentation files from scratch, not just changed files
- **Fresh Start Option**: Perfect for config changes or major repository restructures  
- **Smart Detection**: Automatically identifies full rebuild requests via branch name or PR title
- **Cost Transparency**: Clear token estimation and approval workflow before processing

*Note: Current `wai-docs-update` branch triggers incremental documentation of all repository files. The upcoming full rebuild will delete existing docs and regenerate everything from scratch.*

## 🔗 Get Started Today

[Install AI Document Creator](https://github.com/apps/wagi-docbot) and transform your documentation workflow!

---

Built with ❤️ by WAI · [Website](https://woden-ai.com) · [Pricing](https://woden-ai.com/products) · [Support](mailto:support@woden-ai.com)
