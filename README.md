# Movie Recommender

## Overview

- [video](https://youtu.be/eKmIVU8EUbw)

## Usage

#### Local

#### Cloud

1. Create a [GPU instance](https://aws.amazon.com/) in the US East N. Virginia region using the preconfigured AMI [Amazon Machine Image] called 'ami-d6f2e6bc'.
2. Download this repo. 
3. Upload this repo to the root directory of the GPU instance via FileZilla.
4. SSH into that instance.
5. Compile the project using the following commands:

```bash
cd amazon-dsstne/src/amazon/dsstne
# Add the mpiCC and nvcc compiler in the path
export PATH=/usr/local/openmpi/bin:/usr/local/cuda/bin:$PATH
make
export PATH=`pwd`/bin:$PATH
cd samples
g++ commands.cpp demo.cpp 
./a.out
cpp demo.cpp
```

# Contributors

- [DSSTNE](https://github.com/amznlabs) 
- [Siraj Raval](https://github.com/llSourcell)
- [B. Bueno](https://github.com/bbueno25)