# SINGLETON SD - SCRIPTS - DOCKER

This project contains Linux bash scripts to use with docker.

> The **main repository** is hosted in [gitlab.com/singletonsd/scripts/docker](https://gitlab.com/singletonsd/scripts/docker.git) but it is automaticaly mirrored to [github.com/singletonsd](https://github.com/singletonsd/docker.git), [github.com/patoperpetua](https://github.com/patoperpetua/scripts-docker.git) and to [gitlab.com/patoperpetua](https://gitlab.com/patoperpetua/scripts-docker.git). If you are in the Github page it may occur that is not updated to the last version.

## AVAILABLE SCRIPTS

<!-- TODO: add scripts -->
### docker_build_multiple_images

Generates all docker images contained in a folder named *docker-images*. The project must have the following structure:

```bash
- docker-images
    - base_name
        - Dockerfile
        - tags
    - another_base_name
        - Dockerfile
        - tags
```

Each folder represent a type of image. The folder name will be base name of the generated folder.

The file tags contains the different tags of the base image used. It must contain one tag per line and finished with an empty line. Example:

```bash
8-alpine
10-alpine

```

It has the following available options:

```bash
-h | --help: display help.
-p | --push: push images after building.
-x | --proxy: use proxy.
-b | --base-name: base name of images.
-c | --commit-sha: sha of commit to attach to image.
-t | --tag: tag of images.
```

Also, it can be used envieronment variables:

```bash
DOCKER_BUILD_BASE_NAME=
DOCKER_BUILD_TAG=
```

#### Download

It can be downloaded by:

```bash
curl -o docker_build_multiple_images.sh -L https://singletonsd.gitlab.io/scripts/docker/latest/docker_build_multiple_images.sh
```

## STRUCTURE

Master branch is setup as latest folder. To use an specific version, put the version name before the file name like:

```url
https://singletonsd.gitlab.io/scripts/docker/latest/gitlab-ci_lint_test_standalone.sh
https://singletonsd.gitlab.io/scripts/docker/develop/gitlab-ci_lint_test_standalone.sh
https://singletonsd.gitlab.io/scripts/docker/v0.0.2/gitlab-ci_lint_test_standalone.sh
```

## DOCUMENTATION

- [Shellcheck](https://github.com/koalaman/shellcheck)

## TODO

- [ ] Fix documentation.
- [X] Add script to download test script from gitlab pages.
- [X] Zip all scripts and put inside pages.

----------------------

© [Singleton SD](http://www.singletonsd.com), Italy, 2019.
