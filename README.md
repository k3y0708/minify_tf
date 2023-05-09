# Minify TF

This is a simple script to output minify the Terraform CLI output. The script is **only** able to plan (or plan a destruction) because you should always check the real plan before applying.

## Usage

Normal planning:

```bash
minify_tf plan # Plan the Creation/Update of the infrastructure
minify_tf destroy # Plan the Destruction of the infrastructure
```

Regenerate the last plan:

```bash
minify_tf regen # Regenerate the last plan with minimal output
minify_tf regenfull # Regenerate the last plan with full output
```

Other commands:

```bash
minify_tf about # Show the about message
minify_tf version # Show the version of the script
```

## Installation

There are two ways of installing this script:

1. Put the script in your `$PATH` (e.g. `/usr/local/bin`)
2. Use Homebrew (or Linuxbrew) to install it:

```bash
brew tap k3y0708/tap
brew install k3y0708/tap/minify-tf
```
