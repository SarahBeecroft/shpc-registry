---
layout: container
name:  "quay.io/biocontainers/mob_suite"
maintainer: "@vsoch"
github: "https://github.com/singularityhub/shpc-registry/blob/main/quay.io/biocontainers/mob_suite/container.yaml"
config_url: "https://raw.githubusercontent.com//singularityhub/shpc-registry/main/quay.io/biocontainers/mob_suite/container.yaml"
updated_at: "2022-10-27 00:45:08.494794"
latest: "3.1.0--pyhdfd78af_0"
container_url: "https://biocontainers.pro/tools/mob_suite"
aliases:
 - ".mob_suite-post-link.sh"
 - "mob_cluster"
 - "mob_init"
 - "mob_recon"
 - "mob_typer"
versions:
 - "3.1.0--pyhdfd78af_0"
description: "shpc-registry automated BioContainers addition for mob_suite"
config: {"url": "https://biocontainers.pro/tools/mob_suite", "maintainer": "@vsoch", "description": "shpc-registry automated BioContainers addition for mob_suite", "latest": {"3.1.0--pyhdfd78af_0": "sha256:ea9a68e1fb86f058e4cd42e384a7f51df18689fdd585fa03790ed079733df629"}, "tags": {"3.1.0--pyhdfd78af_0": "sha256:ea9a68e1fb86f058e4cd42e384a7f51df18689fdd585fa03790ed079733df629"}, "docker": "quay.io/biocontainers/mob_suite", "aliases": {".mob_suite-post-link.sh": "/usr/local/bin/.mob_suite-post-link.sh", "mob_cluster": "/usr/local/bin/mob_cluster", "mob_init": "/usr/local/bin/mob_init", "mob_recon": "/usr/local/bin/mob_recon", "mob_typer": "/usr/local/bin/mob_typer"}}
---

This module is a singularity container wrapper for quay.io/biocontainers/mob_suite.
shpc-registry automated BioContainers addition for mob_suite
After [installing shpc](#install) you will want to install this container module:


```bash
$ shpc install quay.io/biocontainers/mob_suite
```

Or a specific version:

```bash
$ shpc install quay.io/biocontainers/mob_suite:3.1.0--pyhdfd78af_0
```

And then you can tell lmod about your modules folder:

```bash
$ module use ./modules
```

And load the module, and ask for help, or similar.

```bash
$ module load quay.io/biocontainers/mob_suite/3.1.0--pyhdfd78af_0
$ module help quay.io/biocontainers/mob_suite/3.1.0--pyhdfd78af_0
```

You can use tab for auto-completion of module names or commands that are provided.

<br>

### Commands

When you install this module, you will be able to load it to make the following commands accessible.
Examples for both Singularity, Podman, and Docker (container technologies supported) are included.

#### mob_suite-run:

```bash
$ singularity run <container>
$ podman run --rm  -v ${PWD} -w ${PWD} <container>
$ docker run --rm  -v ${PWD} -w ${PWD} <container>
```

#### mob_suite-shell:

```bash
$ singularity shell -s /bin/sh <container>
$ podman run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
$ docker run --it --rm --entrypoint /bin/sh  -v ${PWD} -w ${PWD} <container>
```

#### mob_suite-exec:

```bash
$ singularity exec <container> "$@"
$ podman run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
$ docker run --it --rm --entrypoint ""  -v ${PWD} -w ${PWD} <container> "$@"
```

#### mob_suite-inspect:

Podman and Docker only have one inspect type.

```bash
$ podman inspect <container>
$ docker inspect <container>
```

#### mob_suite-inspect-runscript:

```bash
$ singularity inspect -r <container>
```

#### mob_suite-inspect-deffile:

```bash
$ singularity inspect -d <container>
```


#### .mob_suite-post-link.sh

```bash
$ singularity exec <container> /usr/local/bin/.mob_suite-post-link.sh
$ podman run --it --rm --entrypoint /usr/local/bin/.mob_suite-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/.mob_suite-post-link.sh   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mob_cluster

```bash
$ singularity exec <container> /usr/local/bin/mob_cluster
$ podman run --it --rm --entrypoint /usr/local/bin/mob_cluster   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mob_cluster   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mob_init

```bash
$ singularity exec <container> /usr/local/bin/mob_init
$ podman run --it --rm --entrypoint /usr/local/bin/mob_init   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mob_init   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mob_recon

```bash
$ singularity exec <container> /usr/local/bin/mob_recon
$ podman run --it --rm --entrypoint /usr/local/bin/mob_recon   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mob_recon   -v ${PWD} -w ${PWD} <container> -c " $@"
```


#### mob_typer

```bash
$ singularity exec <container> /usr/local/bin/mob_typer
$ podman run --it --rm --entrypoint /usr/local/bin/mob_typer   -v ${PWD} -w ${PWD} <container> -c " $@"
$ docker run --it --rm --entrypoint /usr/local/bin/mob_typer   -v ${PWD} -w ${PWD} <container> -c " $@"
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