# devcontainer-devbox

A template repository to accelerate the creation of devcontainers, primarily for use with GitHub Codespaces.

## Overview

This repository leverages the power of [Devbox](https://www.jetify.com/docs/devbox/cli_reference/devbox_generate_devcontainer/) to
generate customized devcontainers. It offers a pre-configured environment with:

- A curated selection of development tools
- Minor but useful tweaks to the default devcontainer setup
- Ready-to-use configurations for common development scenarios

## Key Features

1. **Curated Tool Selection**: Includes a set of pre-configured tools favored by the author. See [devbox.json](./devbox.json) for
the complete list.

2. **Custom Dockerfile**: The [Dockerfile](.devcontainer/Dockerfile) contains minor enhancements not present in the default
Devbox-generated devcontainer.

3. **Enhanced devcontainer.json**: The [devcontainer.json](.devcontainer/devcontainer.json) file includes customizations for
Docker and SSH feature installation.

## Usage Considerations

- **Initial Build Time**: Due to the inclusion of numerous tools, the first-time build of the devcontainer may take longer than
usual.
- **Pre-build Option**: Consider utilizing GitHub's pre-build capabilities for Codespaces to optimize startup times.

## Getting Started

1. Clone this repository or use it as a template for your new project.
2. Customize the `devbox.json`, Dockerfile, and `devcontainer.json` as needed for your specific project requirements.
3. Use with GitHub Codespaces or your local development environment supporting devcontainers.

## Contributing

Contributions to improve this template are welcome. Please submit issues or pull requests with your suggestions or enhancements.
