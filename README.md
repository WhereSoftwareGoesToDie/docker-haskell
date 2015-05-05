docker-haskell
==============

This builds a Haskell build environment in a Docker image. It uses Stackage for stable builds.

To add additional packages to the build environment, add lines to the following files:

| File                 | Description              |
|----------------------|--------------------------|
| `src/apt-packages`   | Debian packages          |
| `src/yum-packages`   | CentOS packages          |
| `src/cabal-tools`    | Tools (happy, alex, ...) |
| `src/cabal-packages` | Cabal Packages           |


Usage
-----
```
./build $NAME $DOCKER_REGISTRY $DOCKER_OPTS
```
