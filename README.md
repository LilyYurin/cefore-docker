# cefore-docker
Docker image running Cefore on Ubuntu 22.04
The usage is described below.

## Usage
```
# Move to the cloned repository
$ cd cefore-docker

# Build four types of images: cefore/base, cefore/min, cefore/cache, and cefore/csmgr
$ sudo bash ./build.bash 

# Display a list of the built images
$ sudo docker images
```
After the build is complete, the following four images will be generated:
- base: The foundational image.
- min: An image with a minimal configuration.
- cache: An image with a local cache.
- csmgr: An image that includes the csmgr functionality.

Operation has been confirmed with Cefore version 0.11.0 as of May 23, 2025.
