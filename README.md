# Download Convox CLI Buildkite Plugin [![Changelog](https://img.shields.io/badge/-Changelog-blue)](./CHANGELOG.md)

A [Buildkite plugin](https://buildkite.com/docs/agent/v3/plugins) that downloads the Convox CLI and places it into `$PATH`

## Example

The following pipeline will build a new release, downloading the latest Convox CLI first.

```yaml
steps:
  - plugins:
    - liamdawson/download-convox-cli#v1.0.0:
        os: linux
    - liamdawson/convox-build#v1.0.0:
        rack: test-rack
        app: test-app
```
