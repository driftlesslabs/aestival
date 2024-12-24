# aestival
Development Environment for ActivitySim Estimation Mode

The [aestival github repository](https://github.com/driftlesslabs/aestival) 
contains everything needed to set up a development environment for ActivitySim's 
estimation mode, including:

- [ActivitySim](https://github.com/driftlesslabs/activitysim) 
- [Larch](https://github.com/driftlesslabs/larch)
- [Sharrow](https://github.com/driftlesslabs/sharrow)

## Installation

To set everything up, you can run the following commands (mac/linux):

```bash
# Install the pixi.sh CLI (if needed)
curl -fsSL https://pixi.sh/install.sh | bash

# Install the GitHub CLI (if needed)
pixi global install gh

# Clone the repository
gh repo clone driftlesslabs/aestival -- --recurse-submodules

# Set up the development environment and run some tests
cd aestival
pixi run test-core
```

For windows, it's similar, but the pixi install command on the first line is 
different:

```powershell
iwr -useb https://pixi.sh/install.ps1 | iex
```

To clone a particular branch of `aestival`, you can use the following command:

```bash
gh repo clone driftlesslabs/aestival -- --recurse-submodules -b <branch> --single-branch
```
