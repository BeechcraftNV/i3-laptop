# i3-laptop Configuration

This repository contains my personal i3 window manager configuration optimized for laptop use. It includes configurations for i3, i3blocks, and related scripts to streamline the i3 experience on a laptop environment.

## Contents

- `config`: The main i3 configuration file
- `i3blocks.conf`: Configuration for the i3blocks status bar
- `scripts/`: Directory containing helper scripts
  - `setup-monitors.sh`: Script for configuring external monitors
- `switch-to-i3.sh`: Script for switching to i3 window manager

## Prerequisites

To use this configuration, you'll need:

- i3 window manager (i3-wm)
- i3blocks for the status bar
- Any dependencies referenced in the configuration files or scripts

On Ubuntu/Debian-based systems, you can install the required packages with:

```bash
sudo apt update
sudo apt install i3 i3blocks
```

## Installation

### Setting up on a new machine

To clone this repository to a new machine:

```bash
# Back up any existing i3 configuration
mv ~/.config/i3 ~/.config/i3.backup

# Clone the repository
git clone git@github.com:BeechcraftNV/i3-laptop.git ~/.config/i3

# Make scripts executable if needed
chmod +x ~/.config/i3/scripts/*.sh
chmod +x ~/.config/i3/switch-to-i3.sh
```

### Updating an existing installation

If you've already cloned the repository, you can update to the latest version with:

```bash
cd ~/.config/i3
git pull
```

## Usage

### Making changes

After making changes to your configuration:

1. Review your changes:
   ```bash
   git status
   git diff
   ```

2. Commit and push your changes:
   ```bash
   git add .
   git commit -m "Description of your changes"
   git push
   ```

### Handling different machine configurations

If you need to make machine-specific adjustments:

1. Create a file for machine-specific settings
2. Add it to the `.gitignore` file to prevent it from being committed
3. Source or import this file from your main configuration

## .gitignore Setup

The `.gitignore` file is configured to exclude:

- Editor backup files and temporary files
- System-specific files
- Log files
- Files that might contain sensitive information
- Executable binaries and build directories

This ensures that only the essential configuration files are tracked in the repository, while keeping it clean of machine-specific or sensitive data.

## Customization

Feel free to modify any configuration files to suit your specific needs. The i3 configuration is designed to be modular and easily customizable.

## License

This is personal configuration. Feel free to use, modify, and distribute as you see fit.
