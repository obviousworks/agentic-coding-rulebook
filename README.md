# Agentic Coding Rulebook

**The Universal Configuration Standard for AI-Assisted Development**

A comprehensive, production-ready collection of configuration files, templates, and best practices for professional AI-assisted coding across all major AI IDEs and coding assistants.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

## 🎯 What is Agentic Coding?

Agentic coding (also known as vibe coding) is a structured development methodology where developers collaborate with AI agents through explicit rules, context management, and best practices. Instead of blindly trusting AI output, you create a "constitutional framework" that guides AI behavior, ensuring consistent, secure, and maintainable code.

**The Key Principle:** Context is king. AI agents are only as good as the rules and context you provide them.

## 🚀 Why This Repository?

- **Universal Standard**: Based on the 2025 AGENTS.md standard backed by OpenAI, Google, Anthropic, Cursor, and Sourcegraph
- **Tool-Agnostic**: Works across Windsurf, Cursor, GitHub Copilot, Claude Code, and all major AI IDEs
- **Production-Ready**: Battle-tested rules from real-world projects, not academic examples
- **Security-First**: Explicit security guardrails to prevent common AI-generated vulnerabilities
- **Token-Optimized**: Carefully crafted to maximize efficiency and minimize costs
- **Comprehensive**: Covers everything from setup to advanced multi-agent workflows

## 📦 What's Included

### Core Templates
- **`AGENTS.md`** - Universal AI agent configuration (the new standard)
- **`agent_template.md`** - Production-ready template with placeholders
- **`agent_example.md`** - Complete real-world example with best practices

### Tool-Specific Configurations
- **`global_rules.md`** - Windsurf global rules (cross-project standards)
- **`.windsurfrules`** - Windsurf project-specific rules with XML structure
- **`.cursorrules`** - Cursor IDE configuration
- **`.github/copilot-instructions.md`** - GitHub Copilot repository instructions
- **`CLAUDE.md`** - Claude Code specific configuration

### Advanced Resources
- **`security_rules.md`** - Comprehensive security guidelines for AI code generation
- **`performance_rules.md`** - Performance optimization patterns
- **`testing_rules.md`** - Testing standards and patterns
- **`migration_guide.md`** - How to migrate from tool-specific to universal configs

### Helper Tools
- **`adaptation_prompt.txt`** - AI prompt to customize templates for your project
- **`project_analyzer.txt`** - Prompt to analyze existing projects and generate rules
- **`best_practices.md`** - Comprehensive guide to effective agentic coding

## 🎨 Quick Start

### 1. Choose Your Approach

**Option A: Universal AGENTS.md (Recommended)**
```bash
# Copy the universal template
cp agent_template.md AGENTS.md

# Edit for your project
# Then create symbolic links for tool compatibility:
ln -s AGENTS.md .cursorrules
ln -s AGENTS.md CLAUDE.md
ln -s AGENTS.md .windsurfrules
```

**Option B: Tool-Specific Start**
```bash
# For Windsurf
cp global_rules.md ~/your-global-rules-location/
cp .windsurfrules ./your-project/

# For Cursor
cp .cursorrules ./your-project/

# For GitHub Copilot
mkdir -p .github
cp copilot-instructions.md .github/
```

### 2. Customize for Your Project

Use our AI-powered customization prompt:

```bash
# Read adaptation_prompt.txt
# Fill in your project details
# Let AI generate your customized configuration
```

Or use the project analyzer:

```bash
# Read project_analyzer.txt
# Point it at your existing codebase
# Get AI-generated rules based on your patterns
```

### 3. Verify and Test

```bash
# Ask your AI agent to implement a simple feature
# Review if it follows your rules
# Iterate on rule clarity if needed
```

## 🏗️ Repository Structure

```
agentic-coding-rulebook/
├── README.md                          # This file
├── AGENTS.md                          # Universal standard template
├── agent_template.md                  # Customizable template with placeholders
├── agent_example.md                   # Real-world complete example
│
├── tool-specific/
│   ├── windsurf/
│   │   ├── global_rules.md           # Cross-project standards
│   │   ├── .windsurfrules            # Project-specific XML config
│   │   └── windsurfrules_example.md  # Complete example
│   │
│   ├── cursor/
│   │   ├── .cursorrules              # Cursor configuration
│   │   └── cursor_rules_example.md   # Complete example
│   │
│   ├── github-copilot/
│   │   ├── copilot-instructions.md   # Repository instructions
│   │   └── copilot_example.md        # Complete example
│   │
│   └── claude-code/
│       ├── CLAUDE.md                  # Claude Code configuration
│       └── claude_example.md          # Complete example
│
├── specialized-rules/
│   ├── security_rules.md              # Security-first patterns
│   ├── performance_rules.md           # Performance optimization
│   ├── testing_rules.md               # Testing standards
│   └── accessibility_rules.md         # A11y guidelines
│
├── helpers/
│   ├── adaptation_prompt.txt          # Customize template for your project
│   ├── project_analyzer.txt           # Analyze existing projects
│   └── rule_validator.txt             # Validate rule effectiveness
│
├── guides/
│   ├── getting_started.md             # Step-by-step setup guide
│   ├── best_practices.md              # Comprehensive methodology guide
│   ├── migration_guide.md             # Tool migration strategies
│   ├── troubleshooting.md             # Common issues and solutions
│   └── advanced_patterns.md           # Multi-agent, hierarchical configs
│
└── examples/
    ├── react-nextjs-project/          # Full example: React/Next.js
    ├── python-fastapi-project/        # Full example: Python/FastAPI
    ├── java-spring-project/           # Full example: Java/Spring Boot
    └── monorepo-example/              # Full example: Monorepo structure
```

## 🎓 Core Principles

Our rulebook is built on proven principles from production environments:

### 1. **Simplicity First (SF)**
Choose the simplest viable solution. Complex patterns require explicit justification.

### 2. **Readability Priority (RP)**
Code must be immediately understandable by both humans and AI during future modifications.

### 3. **Dependency Minimalism (DM)**
No new libraries or frameworks without explicit request or compelling justification.

### 4. **Security First (SecF)**
All external data validated, no secrets in code, explicit security requirements.

### 5. **Test-Driven Thinking (TDT)**
Design all code to be easily testable from inception.

### 6. **Token Efficiency (TE)**
Use file-scoped commands, reference external docs, optimize context window usage.

## 🔒 Security Considerations

AI-generated code requires explicit security guardrails:

- **Never trust AI output without review** - Treat all generated code as untrusted
- **Validate all inputs** - Explicit validation rules in your configuration
- **No secrets in code** - Environmental variables and secret management
- **Security scanning** - SAST, SCA, secrets detection in CI/CD
- **Explicit security patterns** - Authentication, authorization, encryption requirements

See `specialized-rules/security_rules.md` for comprehensive guidelines.

## ⚡ Performance Optimization

Token efficiency directly impacts costs and speed:

- **File-scoped commands** - `npm run tsc --noEmit path/to/file.tsx` (3 seconds) vs `npm run build` (3 minutes)
- **Target <2,000 tokens** - Start minimal, grow organically
- **Reference, don't duplicate** - Link to external docs instead of embedding
- **Hierarchical organization** - Separate configs for monorepo packages
- **Prompt caching** - Place stable content first

See `specialized-rules/performance_rules.md` for optimization patterns.

## 🛠️ Supported Tools

This rulebook works with all major AI coding assistants:

| Tool | Configuration File | Native Support | Via Symlink |
|------|-------------------|----------------|-------------|
| **Universal** | `AGENTS.md` | ✅ OpenAI Codex, Google Jules, Cursor, Factory AI | - |
| **Windsurf** | `.windsurfrules` or `global_rules.md` | ✅ Native | Via symlink to AGENTS.md |
| **Cursor** | `.cursorrules` or `.cursor/rules/*.mdc` | ✅ Native | Via symlink to AGENTS.md |
| **GitHub Copilot** | `.github/copilot-instructions.md` | ✅ Native + reads AGENTS.md | - |
| **Claude Code** | `CLAUDE.md` | ✅ Native + reads AGENTS.md | Via symlink to AGENTS.md |
| **Aider** | `AGENTS.md` | ✅ Native | - |
| **Zed** | `AGENTS.md` | ✅ Native | - |

## 📚 Documentation

- **[Getting Started Guide](guides/getting_started.md)** - Step-by-step setup for beginners
- **[Best Practices](guides/best_practices.md)** - Comprehensive methodology guide
- **[Migration Guide](guides/migration_guide.md)** - Moving from tool-specific to universal configs
- **[Advanced Patterns](guides/advanced_patterns.md)** - Multi-agent workflows, hierarchical configs
- **[Troubleshooting](guides/troubleshooting.md)** - Common issues and solutions

## 🤝 Contributing

We welcome contributions! See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Ways to contribute:**
- Share your production-ready rule examples
- Improve existing templates with real-world learnings
- Add support for new tools and frameworks
- Report issues or suggest enhancements
- Improve documentation and guides

## 📖 Real-World Success Stories

> "Reduced AI-generated bugs by 70% after implementing these security rules. Game changer for our team." - Senior Engineer at Tech Startup

> "The token optimization tips saved us $2,000/month in API costs. File-scoped commands alone were worth it." - CTO at SaaS Company

> "Finally, consistent code across all our microservices. The hierarchical AGENTS.md approach works perfectly." - Lead Developer at Enterprise

## 🔗 Related Resources

- **[AGENTS.md Official Spec](https://agents.md)** - The universal standard
- **[OpenAI Codex Documentation](https://platform.openai.com/docs/guides/code)** - Official OpenAI guidance
- **[Cursor Documentation](https://docs.cursor.com)** - Cursor IDE rules
- **[GitHub Copilot Custom Instructions](https://docs.github.com/copilot/customizing-copilot)** - Copilot configuration
- **[Windsurf Directory](https://codeium.com/windsurf/directory)** - Windsurf rule examples
- **[Vibe Coding AI Rules](https://github.com/obviousworks/vibe-coding-ai-rules)** - Global and Project specific coding rules

## ⚖️ License

MIT License - See [LICENSE](LICENSE) for details.

## 🙏 Acknowledgments

Built on learnings from thousands of production implementations and contributions from the global agentic coding community. Special thanks to:

- The AGENTS.md standardization initiative (OpenAI, Google, Anthropic)
- The Cursor, Windsurf, and GitHub Copilot teams
- The open-source community sharing real-world patterns
- Early adopters who battle-tested these approaches

## 📮 Contact & Support

- **Issues**: [GitHub Issues](https://github.com/obviousworks/agentic-coding-rulebook/issues)
- **Discussions**: [GitHub Discussions](https://github.com/obviousworks/agentic-coding-rulebook/discussions)
- **Website**: [www.obviousworks.ch](https://www.obviousworks.ch)

---

**Start shipping features faster, not bugs faster.** 🚀

Give AI the rules it needs, get the code quality you deserve.
