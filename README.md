# Awesome Starlark
*A list of awesome things related to the Starlark language*

> This page started as a fork of https://github.com/bazelbuild/starlark/blob/master/users.md
> with the goal of having a page that's easier to maintain, iterate on, and promote.
> The repository above is dedicated to the specification, so it has different requirements.

### Starlark Implementations

There are 3 known implementations of the Starlark language:

*   in Go: https://github.com/google/starlark-go/
*   in Java:
    https://github.com/bazelbuild/bazel/tree/master/src/main/java/net/starlark/java
*   in Rust: https://github.com/facebookexperimental/starlark-rust

### Tools

* [Buildifier](https://github.com/bazelbuild/buildtools): Code formatter &
  linter. It can also apply automated fixes (e.g. remove unused loads).
* [Stardoc](https://skydoc.bazel.build/): Documentation generator.
* [Starlark Online Playground](https://laurent.le-brun.eu/starlark/):
    A web playground for Starlark.
* [Starlark Playground](https://github.com/qri-io/starpg): Starlark Playground
  is a web-based starlark editor. It uses the golang implementation of starlark
  running on a server to present a monaco editor set to python syntax.
* [Moonlark](https://github.com/obazl/moonlark): Starlark parser in C with Lua
  bindings.

### Libraries and extensions

*  [Skycfg](https://github.com/stripe/skycfg) is a library for Starlark to
   generate Protocol Buffer messages.
*  [starlark-go-nethttp](https://github.com/pcj/starlark-go-nethttp) is a wrapper
   around a minimal subset of `net/http package` for use within starlark-go.
*  [Starlet](https://github.com/1set/starlet) is a Go wrapper for the [Starlark in Go](https://github.com/google/starlark-go) that
   simplifies script execution, provides data conversion, and offers useful Starlark libraries and extensions.
*  [Starlight](https://github.com/starlight-go/starlight) is a wrapper around the
   Starlark interpreter in Go.

## Bindings

### Python

*  [python-starlark-go](https://github.com/caketop/python-starlark-go): Python bindings for starlark-go
*  [starlark-pyo3](https://github.com/inducer/starlark-pyo3): Python bindings for starlark-rust

## IDEs

Some IDEs have a [plugin for Bazel](https://bazel.build/install/ide).
Otherwise, consider using a Python mode.

## Users

*  [Bazel](https://github.com/bazelbuild/bazel) is a fast, scalable,
   multi-language and extensible build system. Starlark has been designed for
   Bazel.
*  [Buck2](https://buck2.build/) is a build system from Meta, using
   Starlark in a similar way as Bazel.
*  [Copybara](https://github.com/google/copybara) is a tool for transforming and
   moving code between repositories. It embeds Starlark to configure the workflow.
*  [Delve](https://github.com/go-delve/delve) is a debugger for the Go
   programming language, aiming to provide a simple, full featured debugging
   tool for Go. [Delve uses Starlark](https://github.com/go-delve/delve/blob/master/Documentation/cli/starlark.md)
   as a a scripting language.
*  [Drone](https://drone.io) is a self-service Continuous Delivery platform. It
   supports [Starlark scripting](https://docs.drone.io/starlark/overview/) as an
   alternate to yaml configurations.
*  [envd](https://github.com/tensorchord/envd) is a CLI to build the docker images
   for machine learning development and production environments.
*  [FizzBee](https://fizzbee.io) is a system design language for verifying
   distributed systems in cloud, micro-services, and event-driven applications.
   It uses Starlark to offer an intuitive, Python-like syntax, making it
   accessible for everyday software developers. 
*  [Isopod](https://github.com/cruise-automation/isopod) created by Cruise
   Automation is a DSL framework for Kubernetes configuration. It renders
   Kubernetes objects as Protocol Buffers.
* [Kurtosis](https://github.com/kurtosis-tech/kurtosis) is a developer tool
   for engineers to package and run environments of containerized services for
   development, testing, and production. Starlark is used as the DSL for
   defining those environments in a deterministic, portable, and readable way,
   without compromising usability for complex cases.
*  [lucicfg](https://chromium.googlesource.com/infra/luci/luci-go/+/refs/heads/master/lucicfg/doc/README.md)
   from Chromium CI is a tool for generating low-level configuration files from Starlark.
*  [Pixlet](https://github.com/tidbyt/pixlet) is a runtime and UX toolkit for generating animations for small LED displays, such as [Tidbyt](https://tidbyt.com/). Starlark is used to write applets whose outputs are WebP animations.
*  [qri](http://qri.io/) is versioned, scriptable, exportable,
   collaborative datasets. It uses Starlark to [describe transformations](https://qri.io/docs/reference/starlark_syntax/).
*  [recur](https://github.com/dbohdan/recur) is a command-line tool that
   retries a command with exponential backoff plus jitter to mitigate the
   thundering herd problem. The success condition is written as a Starlark
   expression.
*  [Tilt](https://tilt.dev/) manages local development instances for teams that
   deploy to Kubernetes. [Tilt files](https://docs.tilt.dev/tiltfile_concepts.html)
   are written in Starlark.
*  [Vela](https://go-vela.github.io/docs/) is a continuous integration and delivery platform.
   It supports [Starlark scripting](https://go-vela.github.io/docs/templates/tutorials/starlark/)
   as an alternative to YAML.
*  [ytt](https://get-ytt.io/) is a templating tool, built on top of Starlark,
   that understands YAML structure allowing you to focus on your data instead of
   how to properly escape it. Read also [IBM's blog post](
   https://developer.ibm.com/blogs/yaml-templating-tool-to-simplify-complex-configuration-management/)
   about it.
