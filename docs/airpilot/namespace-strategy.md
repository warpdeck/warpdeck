# AirPilot Namespace Strategy

This document outlines the comprehensive namespace security strategy implemented for the AirPilot project across multiple package distribution platforms.

## Overview

AirPilot has secured the `airpilot` namespace across three major platforms to ensure consistent branding and prevent namespace squatting:

- **VSCode Extension Store**: AirPilot VSCode Extension
- **npm Registry**: Node.js/JavaScript ecosystem
- **PyPI**: Python Package Index

## Platform Coverage

### VSCode Extension Store

The primary AirPilot VSCode extension is published as `airpilot` on the Visual Studio Code Extension Marketplace.

### npm Registry

**Package Name**: `airpilot`
**Version**: 0.0.1 (placeholder)
**Commands**: `airpilot`, `air`
**Installation**: `npm install -g airpilot`

The npm package serves as a placeholder to reserve the namespace for future Node.js/TypeScript components of the AirPilot platform.

### PyPI (Python Package Index)

**Package Name**: `airpilot`
**Version**: 0.0.1 (placeholder)
**Commands**: `airpilot`, `air`
**Installation**: `pip install airpilot` or `uv tool install airpilot`

The PyPI package reserves the namespace for the planned commercial CLI component.

## Command Aliases

Both npm and PyPI packages provide dual command aliases:

- **`airpilot`**: Full brand name command
- **`air`**: Short, convenient alias

This allows users to choose between the descriptive full name or the quick shorthand.

## Placeholder Functionality

Both placeholder packages provide professional CLI interfaces with:

- **Help system**: `--help` / `-h` flags
- **Version information**: `--version` / `-v` flags
- **Coming soon messaging**: Clear indication of future functionality
- **Repository links**: Direct users to GitHub for updates

## Installation Testing

The packages are designed to work independently. Users should install either the npm OR Python package, not both globally, to avoid command conflicts.

### npm Installation Test

```bash
npm install -g airpilot
air --help
airpilot --version
npm uninstall -g airpilot
```

### Python Installation Test

```bash
uv tool install airpilot
air --help
airpilot --version
uv tool uninstall airpilot
```

## License Strategy

- **VSCode Extension**: Elastic License 2.0 (free to use, restrictions on redistribution)
- **npm Package**: Elastic License 2.0 (placeholder, same terms)
- **PyPI Package**: Elastic License 2.0 (placeholder, will become commercial)

## Future Architecture

The namespace strategy supports the planned dual-tier architecture:

1. **Free Tier**: VSCode Extension (Elastic License 2.0)
2. **Commercial Tier**: Python CLI with license key system (Proprietary)
3. **Optional**: Node.js components for web integration (TBD)

## Rationale

### Multi-Platform Coverage

Securing namespaces across multiple ecosystems ensures:

- **Brand protection**: Prevents namespace squatting
- **User choice**: Allows installation via preferred package manager
- **Ecosystem compatibility**: Supports both Python and Node.js workflows
- **Future flexibility**: Enables expansion into either ecosystem

### Dual Command Strategy

Providing both `airpilot` and `air` commands offers:

- **Accessibility**: Short command for frequent use
- **Clarity**: Full name for documentation and discovery
- **Professional polish**: Demonstrates attention to user experience

## Maintenance

The placeholder packages require minimal maintenance:

- **Version updates**: Sync versions across platforms when releasing
- **Link updates**: Ensure repository and contact information stays current
- **License alignment**: Keep license terms consistent with main project

## Next Steps

1. **Development**: Build actual CLI functionality for Python package
2. **Migration**: Replace placeholder with commercial Python CLI
3. **Integration**: Develop VSCode extension integration with CLI
4. **Documentation**: Expand user guides and API documentation
