# Playground

Welcome to `playground`, a Swift script that enables you to super quickly generate Swift playgrounds from the command line - with or without dependencies - for any supported platform.

**Features**

- [X] Generate playgrounds in seconds.
- [X] Automatically reuse any playground created today, for easy code note taking.
- [X] Add dependencies to a playground with a simple command - no more fiddling with workspaces.
- [X] Supports iOS, macOS & tvOS.

## Usage

**Simply run `playground` and a new playground will be created and opened**

```
$ playground
```

You can also supply various arguments to customize your playground:

**Add a playground at a specific path**

```
$ playground -t ~/MyPlayground
```

**Add some dependencies to your playground**

```
$ playground -d ~/unbox/unbox.xcodeproj,~/files/files.xcodeproj
```

**Specify what platform you want the playground to run on**

```
$ playground -p tvOS
```

*For all available options, run `$ playground -h`*

## Installation

The easiest way to install `playground` is using [Marathon](https://github.com/johnsundell/marathon):

```
$ marathon install https://raw.githubusercontent.com/JohnSundell/Playground/master/Sources/Playground.swift
```

You can also install it using the Swift Package Manager:

```
$ git clone git@github.com:JohnSundell/Playground.git
$ cd Playground
$ swift build -c release -Xswiftc -static-stdlib
$ cp -f .build/release/Playground /usr/local/bin/playground
```

## Help, feedback or suggestions?

- [Open an issue](https://github.com/JohnSundell/Playground/issues/new) if you need help, if you found a bug, or if you want to discuss a feature request.
- [Open a PR](https://github.com/JohnSundell/Playground/pull/new/master) if you want to make some change to `playground`.
- Contact [@johnsundell on Twitter](https://twitter.com/johnsundell) for discussions, news & announcements about `playground` & other projects.
