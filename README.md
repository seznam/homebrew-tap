# Seznam.cz Homebrew Tap

[Homebrew](https://brew.sh/) casks for open-source tools published by Seznam.cz.

## Casks

| Cask | Description | Project |
| --- | --- | --- |
| `jailoc` | Run coding agents in sandboxed libkrun micro-VMs | [seznam/jailoc](https://github.com/seznam/jailoc) |

## Requirements

- [Homebrew](https://docs.brew.sh/Installation) on macOS or Linux.
- Platform requirements of each cask. `jailoc` supports macOS on Apple silicon (arm64) and Linux on amd64 and arm64. On Linux it needs read-write access to `/dev/kvm` and a kernel with Landlock (5.19 or later). Docker is optional and only used to build images.

## Installation

Install a cask directly:

```sh
brew install --cask seznam/tap/jailoc
```

Or add the tap first and then install by name:

```sh
brew tap seznam/tap
brew install --cask jailoc
```

Upgrade to the latest release:

```sh
brew update
brew upgrade --cask jailoc
```

## Uninstallation

```sh
brew uninstall --cask jailoc
brew untap seznam/tap
```

## Contributing

The casks in this repository are generated and updated by the release pipeline of each project (with [GoReleaser](https://goreleaser.com/)). Do not edit them by hand, because the next release overwrites the change.

To report a problem with a cask or propose a change, open an issue or a pull request in the source project, for example [seznam/jailoc](https://github.com/seznam/jailoc). Changes to this README or the other repository documents are welcome as pull requests here.

## Security

See [SECURITY.md](SECURITY.md).

## License

[MIT](LICENSE.md), Copyright (c) 2026 Seznam.cz, a.s. Each packaged project is distributed under its own license.
