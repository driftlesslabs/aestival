# ActivitySim Development Environment for Estimation Mode

The [aestival github repository](https://github.com/driftlesslabs/aestival) 
contains everything needed to set up a development environment for ActivitySim's 
estimation mode, including:

- [ActivitySim](https://github.com/driftlesslabs/activitysim) 
- [Larch](https://github.com/driftlesslabs/larch)
- [Sharrow](https://github.com/driftlesslabs/sharrow)

## Installation

To set everything up, you can run the following commands:

```bash
# Install the pixi.sh CLI (if needed)
curl -fsSL https://pixi.sh/install.sh | bash

# Clone the repository
gh repo clone driftlesslabs/aestival -- --recurse-submodules

# Set up the development environment
cd aestival
pixi update
```



## Run tests

To run some ActivitySim tests, you can use the following command:

```bash
pixi run test-core
``` 



## Building the Documentation

To build *this* documentation, you can run the following command from the root 
of this repository:

```bash
pixi run aestival-docs
```

To build *ActivitySim*'s documentation, you can run the following command instead:

```bash
pixi run make-docs
```
