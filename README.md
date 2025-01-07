# devcontainer-devbox

A repository for building and publishing a customized devcontainer image with Gustavo's preferred tools, optimized for GitHub
Codespaces.

## Overview

This project uses [Devbox](https://www.jetify.com/docs/devbox/cli_reference/devbox_generate_devcontainer/) to create a tailored
development environment with pre-configured tools and enhancements.

## Key Features

- Curated tool selection in [devbox.json](./devbox.json)
- Enhanced [Dockerfile](.devcontainer/Dockerfile) and [devcontainer.json](.devcontainer/devcontainer.json)

## Usage

To use this image in your devcontainer:

```json
{
  "image": "ghcr.io/garodriguezlp/devcontainer-devbox/devcontainer:latest"
}
```

## Building and Publishing

This repository uses `devcontainers/ci@v0.3` for image management.

## Contributing

Contributions are welcome via issues or pull requests.
