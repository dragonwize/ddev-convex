[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/dragonwize/ddev-convex/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/dragonwize/ddev-convex/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/dragonwize/ddev-convex)](https://github.com/dragonwize/ddev-convex/commits)
[![release](https://img.shields.io/github/v/release/dragonwize/ddev-convex)](https://github.com/dragonwize/ddev-convex/releases/latest)

# DDEV Convex

## Overview

This add-on integrates Convex into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get dragonwize/ddev-convex
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Convex |
| `ddev logs -s convex` | Check Convex logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.convex --convex-docker-image="ddev/ddev-utilities:latest"
ddev add-on get dragonwize/ddev-convex
ddev restart
```

Make sure to commit the `.ddev/.env.convex` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `CONVEX_DOCKER_IMAGE` | `--convex-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@dragonwize](https://github.com/dragonwize)**
