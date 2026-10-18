# CAMS Example: Harbor & Coastal Autonomous Security

This repository is an independent consumer of the `@oml/cams` methodology package, published to the local registry.

## Overview

The model demonstrates Collaborative Autonomy Management Systems (CAMS) applied to coastal harbor defense:
- **Authority**: Coastal Defense Commander defines high-priority perimeter security intents with sea state and ROE constraints.
- **Mission**: Harbor Coastal Security Mission 2026 defining objectives and probability of success thresholds.
- **Platform**: Coastal Autonomous Task Group comprising autonomous assets (Protector USV-1 and ScanEagle UAV-1) providing surface patrol and persistent EO/IR sensing capabilities.
- **Engagement**: Coastal Harbor Defense Engagement Plan containing the Harbor Entrance & Perimeter Patrol OPM, allocating roles to assets and evaluating success probabilities.
- **Playbook Generation**: Generated operational playbook via installed `@oml/cams/codegen/playbook`.

## Usage

```bash
# Install dependencies from registry
oml install --registry http://localhost:4873/

# Start server, lint, validate, and reason
oml start
oml lint
oml validate
oml reason

# Generate the autonomous playbook
oml codegen -c coastalPlaybook
```
