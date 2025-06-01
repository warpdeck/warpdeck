# AirPilot Documentation

Welcome to the AirPilot documentation directory. This contains comprehensive documentation for the AirPilot project architecture, implementation details, and strategic decisions.

## Documentation Index

### Strategic Planning Documents

- **[Project Vision Briefing](project-vision-briefing.md)** - Complete evolution from VSCode tool to universal AI rules platform across all knowledge domains. Includes technical roadmap, business model, and expansion strategy for legal, medical, creative, and business applications.

- **[Vertical Strategy and Market Validation](vertical-strategy-and-market-validation.md)** - Comprehensive strategy for targeting specific industry verticals with validated enterprise customers. Covers telco RFP (Cello Group), construction RFP (South Base $2M pain point), and legal verticals with forward-deployed consulting model.

- **[Strategic Implementation Status](strategic-implementation-status.md)** - Current status update on four critical strategic questions: internal validation timeline, South Base deployment, IP ownership alignment, and resource allocation challenges. Documents 60-70 hour weeks and need for immediate team expansion.

- **[Complete AI Infrastructure Ecosystem](complete-ai-infrastructure-ecosystem.md)** - Reveals the full technology stack: AirPilot (conversational workflow development) + Warp Flow (LangGraph/LangChain production platform) + evaluation frameworks. Includes licensing strategy (MIT for Warp Flow, SaaS for AirPilot) and competitive moats through proprietary industry datasets.

### Technical Implementation

- **[Namespace Strategy](namespace-strategy.md)** - Comprehensive overview of namespace security across VSCode Extension Store, npm, and PyPI platforms with dual command aliases (`airpilot`/`air`).

- **[Placeholder Implementation](placeholder-implementation.md)** - Detailed technical documentation of npm and PyPI placeholder packages with professional CLI interfaces and help systems.

## Project Structure

AirPilot is organized as a multi-platform project with the following components:

### Core Components

- **VSCode Extension** (`/src/`) - Main extension code in TypeScript
- **Package Placeholders** - Namespace reservation packages
  - **npm placeholder** (`/npm-placeholder/`) - Node.js ecosystem
  - **PyPI placeholder** (`/pypi-placeholder/`) - Python ecosystem

### Supporting Directories

- **Documentation** (`/docs/`) - This directory
- **Plans** (`/plans/`) - Project planning and design documents
- **Memory Bank** (`/memory-bank/`) - Project context and progress tracking
- **Assets** (`/assets/`) - Visual assets and branding materials

## Getting Started

### For Contributors

1. Review the [Namespace Strategy](namespace-strategy.md) to understand the multi-platform approach
2. Read [Placeholder Implementation](placeholder-implementation.md) for technical details
3. Check the `/plans/` directory for current development roadmap

### For Users

- **VSCode Extension**: Install from the Extension Marketplace
- **CLI Preview**: Install placeholder via `npm install -g airpilot` or `uv tool install airpilot`

## Architecture Overview

AirPilot has evolved into a complete AI infrastructure ecosystem:

### Three-Component Architecture

- **AirPilot**: Conversational workflow development and capture ($5-8/month SaaS + Enterprise licensing)
- **Warp Flow**: Visual production platform with LangGraph/LangChain (MIT licensed, open source)
- **Evaluation Framework**: Proprietary industry datasets and benchmarks (competitive moat)

### Revenue Model

- **Consumer SaaS**: AirPilot subscriptions for individuals and small teams
- **Enterprise Consulting**: Forward-deployed engagements (South Base $2M RFP optimization)
- **Platform Services**: Training, support, and custom implementations
- **Marketplace**: Vertical-specific rule templates and industry benchmarks

## Key Discussion Points for CEO Meeting

### Immediate Decisions Needed

1. **Resource Allocation**: Funding for 1-2 additional technical team members (60-70 hour weeks unsustainable)
2. **South Base Engagement**: Final pricing and scope for end-of-June deployment
3. **Open Source Timeline**: When to release Warp Flow under MIT license
4. **Investment Strategy**: Budget allocation for AirPilot development and team expansion

### Strategic Opportunities

1. **Andrew Allen's Portfolio**: Multi-company AI implementation across business ecosystem
2. **Vertical Expansion**: Construction → Legal → Additional industries through proven model
3. **Evaluation Competitive Moat**: Proprietary datasets from each engagement create sustainable advantages
4. **Consumer-to-Enterprise Pipeline**: SaaS subscriptions generate enterprise leads and market validation

## Namespace Security

The project secures the `airpilot` brand across three major platforms:

1. **VSCode Extension Store** - Primary extension platform
2. **npm Registry** - JavaScript/Node.js ecosystem
3. **PyPI** - Python Package Index

Both npm and PyPI packages provide dual commands (`airpilot` and `air`) for user convenience.

## Contributing

When contributing to documentation:

1. Follow the established markdown formatting standards
2. Maintain consistency with existing documentation style
3. Include relevant code examples and command snippets
4. Update this index when adding new documentation files

## License

- **Documentation**: Elastic License 2.0
- **VSCode Extension**: Elastic License 2.0
- **Placeholders**: Elastic License 2.0
- **Future CLI**: Will be commercial/proprietary

For detailed license information, see the LICENSE file in the project root.

## Contact

- **Repository**: <https://github.com/shaneholloman/airpilot>
- **Issues**: <https://github.com/shaneholloman/airpilot/issues>
- **Maintainer**: Shane Holloman
