# Prebuilds

This repository contains GitHub Actions and Releases to prebuild software for installation.

## Information

### Dependencies

Helpers for code quality are located in `bin/helpers`

- `brew install shellcheck`
- `brew install focusaurus/homebrew-shfmt/shfmt`

### Containers

- fedora `public.ecr.aws/amazonlinux/amazonlinux:2022`
- ubuntu `public.ecr.aws/lts/ubuntu:jammy`

### Platforms

- x86_64 `linux/amd64`
- arm64 `linux/arm64`

### NodeJS versions

- 14
- 16
- 18

### Python versions

- 3.7
- 3.8
- 3.9
- 3.10
- 3.11

### Docker commands

- interactive `docker run --platform <platform> --entrypoint /bin/bash -it -v "$(pwd):/var/task" --rm <image>`
- command `docker run --platform <platform> --entrypoint "/bin/bash" -v "$(pwd):/var/task" --rm <image> -c "<bash-commands>"`
