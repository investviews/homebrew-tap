# Investviews Homebrew tap

Homebrew packages for InvestViews tools.

## Install

```sh
brew install investviews/tap/investviews
```

Or tap first, then install:

```sh
brew tap investviews/tap
brew install investviews
```

Then authenticate and try it:

```sh
investviews auth login --token <your-token>
investviews geo search "ruzafa valencia"
```

Docs: <https://docs.investviews.ai>

## What is in here

| path | what it is |
|---|---|
| `Casks/investviews.rb` | the `investviews` CLI — [Investviews/investviews-cli](https://github.com/Investviews/investviews-cli) |

## ⚠️ Do not hand-edit the casks

Everything under `Casks/` is **generated and committed by GoReleaser** when a `v*` tag is pushed in
the source repository. A manual edit is overwritten by the next release without warning, and in the
meantime it describes a build nobody can reproduce.

To change what a cask contains, change `.goreleaser.yaml` in the source repo and cut a release.

Casks, not formulae: Homebrew installs casks on macOS only. Linux users install from the release
tarballs attached to each GitHub release.
