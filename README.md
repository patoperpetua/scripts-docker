# SINGLETON SD - SCRIPTS - DOCKER

This project contains Linux bash scripts to use with docker.

> The **main repository** is hosted in [gitlab.com/singletonsd/scripts/docker](https://gitlab.com/singletonsd/scripts/docker.git) but it is automaticaly mirrored to [github.com/singletonsd](https://github.com/singletonsd/docker.git), [github.com/patoperpetua](https://github.com/patoperpetua/scripts-docker.git) and to [gitlab.com/patoperpetua](https://gitlab.com/patoperpetua/scripts-docker.git). If you are in the Github page it may occur that is not updated to the last version.

## AVAILABLE SCRIPTS

<!-- TODO: add scripts -->

### GITLAB-CI LINT TEST

You can test your .gitlab-ci.yml files by executing the following:

```bash
curl -s https://singletonsd.gitlab.io/scripts/gitlab-ci/latest/gitlab-ci_lint_test_standalone.sh | bash /dev/stdin
```

That script contains the following options:

```bash
-h | --help: display help.
-o | --only: the name of the file or folder to test.
```

Also you can download the script by:

```bash
curl -o gitlab-ci_lint_test_standalone.sh -L https://singletonsd.gitlab.io/scripts/gitlab-ci/latest/gitlab-ci_lint_test_standalone.sh
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
- [ ] Zip all scripts and put inside pages.

----------------------

© [Singleton SD](http://www.singletonsd.com), Italy, 2019.
