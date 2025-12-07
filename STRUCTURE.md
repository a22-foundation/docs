# A22 Documentation Structure

This repository is the **source of truth** for all A22 documentation.

## Purpose

The `docs` repository contains:
- **Guiding Principles** - Core design philosophy
- **Specification v1.0** - Complete language specification
- **Grammar v1.0** - Formal EBNF grammar
- **Tutorials** - Getting started guides
- **API Documentation** - Reference documentation
- **Blog** - Announcements and updates

## Architecture

```
docs/
├── docs/                    # Markdown documentation
│   ├── guiding-principles.md
│   ├── specification-v1.0.md
│   ├── grammar-v1.0.md
│   ├── intro.md
│   └── tutorial-basics/
├── blog/                    # Blog posts
├── src/                     # Docusaurus components
├── static/                  # Static assets
└── docusaurus.config.ts     # Site configuration
```

## Consumption

This repository is designed to be consumed by multiple frontends:

### 1. **Docusaurus Site** (this repo)
- Run locally: `npm run start`
- Build: `npm run build`
- Deploy: Configured for GitHub Pages

### 2. **Astro Static Site** (web repo)
- Uses this repo as a git submodule
- Transforms markdown to Starlight pages
- Optimized for performance and SEO

### 3. **IDE Extensions**
- Can reference markdown directly
- Provides inline documentation

### 4. **CLI Tools**
- Can parse and validate against spec
- Reference implementation can use spec programmatically

## Using as a Submodule

To use this documentation in another project:

```bash
# Add as submodule
git submodule add https://github.com/a22-foundation/docs.git docs

# Initialize and update
git submodule update --init --recursive

# Pull latest changes
cd docs
git pull origin main
cd ..
git add docs
git commit -m "Update docs submodule"
```

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## Governance

See [GOVERNANCE.md](./GOVERNANCE.md) for decision-making process.

## License

Documentation is licensed under Creative Commons Attribution 4.0 International (CC BY 4.0).

Code examples in documentation are licensed under Apache 2.0.
