# Paper template

## Compile the PDF locally

[Install pixi](https://pixi.sh/dev/#installation). Run

```sh
pixi r compile
```

Note that this needs the [GitHub CLI](https://github.com/cli/cli#installation) to be logged in (configuration stored in `~/.config/gh`) and access to the [`zenglib` repository](https://github.com/jinzhezenggroup/zenglib).

## Compile using the GitHub Actions

PDF is built automatically in GitHub Actions for each commit.

### PDF Release on GitHub

When you create a release by pushing a tag, the workflow automatically uploads the generated PDF to the GitHub release:

```sh
git tag v1.0.0
git push origin v1.0.0
```

The PDF will be attached as an asset to the release.
