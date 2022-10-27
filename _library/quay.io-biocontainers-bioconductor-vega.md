---
layout: container
name:  "quay.io/biocontainers/bioconductor-vega"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/bioconductor-vega/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/bioconductor-vega/container.yaml"
updated_at: "2022-10-27 00:19:03.959010"
latest: "1.35.0--r40h037d062_0"
container_url: "https://biocontainers.pro/tools/bioconductor-vega"

versions:
 - "1.35.0--r40h037d062_0"
description: "shpc-registry automated BioContainers addition for bioconductor-vega"
config: {"url": "https://biocontainers.pro/tools/bioconductor-vega", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for bioconductor-vega", "latest": {"1.35.0--r40h037d062_0": "sha256:731284acce192f696bb01e4144d1f16261ca1144a8e6f119a0b6526189c98e5b"}, "tags": {"1.35.0--r40h037d062_0": "sha256:731284acce192f696bb01e4144d1f16261ca1144a8e6f119a0b6526189c98e5b"}, "docker": "quay.io/biocontainers/bioconductor-vega"}
---

This module is a singularity container wrapper for quay.io/biocontainers/bioconductor-vega.
shpc-registry automated BioContainers addition for bioconductor-vega
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/bioconductor-vega
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/bioconductor-vega:1.35.0--r40h037d062_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/bioconductor-vega/1.35.0--r40h037d062_0
$ module help quay.io/biocontainers/bioconductor-vega/1.35.0--r40h037d062_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### bioconductor-vega-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-vega-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### bioconductor-vega-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### bioconductor-vega-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### bioconductor-vega-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### bioconductor-vega-inspect-deffile:

```bash
$ singularity inspect -d <container>
```



#### bioconductor-vega

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```


In the above, the `<container>` directive will reference an actual container provided
by the module, for the version you have chosen to load. An environment file in the
module folder will also be bound. Note that although a container
might provide custom commands, every container exposes unique exec, shell, run, and
inspect aliases. For anycommands above, you can export:

 - SINGULARITY_OPTS: to define custom options for singularity (e.g., --debug)
 - SINGULARITY_COMMAND_OPTS: to define custom options for the command (e.g., -b)
 - PODMAN_OPTS: to define custom options for podman or docker
 - PODMAN_COMMAND_OPTS: to define custom options for the command

<br>

### Install

You can install shpc locally (for yourself or your user base) as follows:

```bash
$ git clone https://github.com/singularityhub/singularity-hpc
$ cd singularity-hpc
$ pip install -e .
```

Have any questions, or want to request a new module or version? [ask for help!](https://github.com/singularityhub/singularity-hpc/issues)