# Placeholder Package Implementation

This document details the implementation of placeholder packages for namespace reservation on npm and PyPI.

## Overview

Two placeholder packages were created to secure the `airpilot` namespace:

- **npm placeholder**: Node.js/JavaScript ecosystem
- **PyPI placeholder**: Python ecosystem

Both packages provide identical user experiences while using platform-appropriate technologies.

## npm Placeholder

### File Structure

```tree
npm-placeholder/
├── package.json          # npm package configuration
├── index.js             # CLI entry point with argument handling
└── README.md            # Package documentation
```

### Key Features

- **Dual commands**: Both `airpilot` and `air` binaries
- **Professional CLI**: Help, version, and default messaging
- **Cross-platform**: Works on Windows, macOS, Linux
- **Zero dependencies**: Lightweight implementation

### package.json Configuration

```json
{
  "name": "airpilot",
  "version": "0.0.1",
  "description": "Universal AI Rules Pilot",
  "bin": {
    "airpilot": "./index.js",
    "air": "./index.js"
  }
}
```

### npm CLI Implementation

The `index.js` file provides:

- Argument parsing for `--help`, `--version` flags
- Professional help output with usage information
- Version display with placeholder notation
- Default "coming soon" messaging
- Repository and contact information

## PyPI Placeholder

### PyPI File Structure

```tree
pypi-placeholder/
├── pyproject.toml              # Modern Python packaging configuration
├── README.md                   # Package documentation
└── src/
    └── airpilot/
        ├── __init__.py         # Package initialization
        └── cli.py              # CLI entry point
```

### PyPI Key Features

- **Modern packaging**: Uses `pyproject.toml` with hatchling
- **uv compatibility**: Optimized for modern Python tooling
- **Dual entry points**: Both `airpilot` and `air` commands
- **Professional CLI**: Matches npm package functionality

### pyproject.toml Configuration

```toml
[build-system]
requires = ["hatchling"]
build-backend = "hatchling.build"

[project.scripts]
airpilot = "airpilot.cli:main"
air = "airpilot.cli:main"
```

### Python CLI Implementation

The `cli.py` file provides:

- Argument parsing using `sys.argv`
- Identical help and version output to npm package
- Consistent user experience across platforms
- Professional error handling

## Shared Design Principles

### Consistent User Experience

Both packages provide identical command-line interfaces:

```bash
# Help system
airpilot --help
air -h

# Version information
airpilot --version
air -v

# Default behavior
airpilot
air
```

### Professional Messaging

All output includes:

- Clear branding: "AirPilot - Universal AI Rules Pilot"
- Placeholder indication: Explicit "coming soon" messaging
- Repository links: Direct users to GitHub for updates
- Contact information: Maintainer details
- Usage hints: Guide users to help system

### No Emoji Policy

Following project standards, all text output uses plain text alternatives:

- No emoji characters in any output
- Professional, clean messaging
- Accessibility-focused design

## Build and Publish Process

### npm Package

```bash
cd npm-placeholder
npm pack --dry-run          # Verify package contents
npm publish --dry-run       # Test publish process
npm publish                 # Publish to npm registry
```

### PyPI Package

```bash
cd pypi-placeholder
uv sync                     # Install dependencies
uv build                    # Build distribution files
uv publish                  # Publish to PyPI
```

## Testing Procedures

### Individual Package Testing

Each package was tested in isolation to prevent command conflicts:

```bash
# Test npm package
npm install -g airpilot
air --help
airpilot --version
npm uninstall -g airpilot

# Test PyPI package
uv tool install airpilot
air --help
airpilot --version
uv tool uninstall airpilot
```

### Verification Points

- Command availability after installation
- Help system functionality
- Version display accuracy
- Clean uninstallation
- No residual files or conflicts

## Troubleshooting

### Troubleshooting Common Issues

1. **Command conflicts**: Installing both packages globally creates conflicts
   - **Solution**: Use only one package at a time globally
   - **Prevention**: Document mutually exclusive installation

2. **Permission errors**: Global installation may require elevated privileges
   - **Solution**: Use `sudo` on Unix systems or administrator prompt on Windows
   - **Alternative**: Use user-scoped installation where supported

3. **Build failures**: PyPI package initially had configuration issues
   - **Solution**: Simplified hatchling configuration
   - **Fix**: Removed invalid classifiers, corrected source mapping

### Debugging Commands

```bash
# Check global installations
npm list -g --depth=0
uv tool list

# Verify command paths
which air
which airpilot

# Test package contents
npm pack --dry-run
uv build
```

## Maintenance Considerations

### Version Synchronization

- Keep versions synchronized across npm and PyPI
- Update placeholder content when main project evolves
- Maintain consistent messaging and links

### License Alignment

- Both packages use Elastic License 2.0
- License terms must stay aligned with main project
- Update license references when project license changes

### Link Maintenance

- Repository URLs must stay current
- Contact information should be updated as needed
- Issue tracker links should remain functional

## Future Migration

### npm Package Migration Strategy

The npm placeholder can be replaced with:

- TypeScript/Node.js CLI implementation
- Web-based components for browser integration
- Development tools and utilities

### PyPI Package Evolution Plan

The PyPI placeholder will become:

- Commercial CLI with license key system
- Advanced configuration management
- API and automation capabilities

Both packages provide clean foundations for future development while securing critical namespace real estate.
