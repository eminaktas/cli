<h1 align="center">KCL CLI</h1>

<p align="center">
<a href="./README.md">English</a> | <a href="./README-zh.md">简体中文</a>
</p>
<p align="center">
<a href="#introduction">Introduction</a> | <a href="#installation">Installation</a> | <a href="#quick-start">Quick start</a> 
</p>

<p align="center">
<img src="https://coveralls.io/repos/github/kcl-lang/cli/badge.svg">
<img src="https://img.shields.io/badge/license-Apache--2.0-green">
<img src="https://img.shields.io/badge/PRs-welcome-brightgreen">
</p>

## Introduction

`kcl` is a command-line interface that includes language core features, IDE features, package management tools, community integration, and other tools.

## Installation

### Scripts

### Go install

You can download `kcl` via `go install`.

```shell
go install kcl-lang.io/cli/cmd/kcl@latest
```

### Download from GITHUB Release Page

You can also get `kcl` from the github release and set the binary path to the environment variable PATH.

```shell
# KCL_CLI_INSTALLATION_PATH is the path of the `KCL CLI` binary.
export PATH=$KCL_CLI_INSTALLATION_PATH:$PATH  
```

Use the following command to ensure that you install `kcl` successfully.

```shell
kcl --help
```

### Build from Source Code

```shell
git clone https://github.com/kcl-lang/cli
cd cli && go build ./cmd/kcl/main.go -o kcl
```

## Quick Start

```shell
kcl run ./examples/kubernetes.k
```

## Frequently Asked Questions (FAQ)

### Q: I am using `go install` to install `kcl`, but I get the error `command not found`.

- A: `go install` will install the binary file to `$GOPATH/bin` by default. You need to add `$GOPATH/bin` to the environment variable `PATH`.

## Learn More

- [KCL Website](https://kcl-lang.io)
