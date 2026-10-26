# setup-nickel

A GitHub Action that installs [Nickel][] and puts it on the `PATH` for
every later step in the job.

## Usage

```yaml
steps:
  - uses: mboes/setup-nickel@v1
    with:
      version: 1.18.0   # optional; defaults to "latest"
  - run: nickel export config.ncl
```

## Inputs

| Name      | Default  | Description                                         |
|-----------|----------|-----------------------------------------------------|
| `version` | `latest` | A Nickel release, such as `1.18.0`, or `latest`.    |

## Outputs

| Name      | Description                        |
|-----------|------------------------------------|
| `version` | The Nickel version installed.      |

## Supported runners

- Linux (x64, ARM64)
- macOS (ARM64)
- Windows (x64)

[nickel]: https://nickel-lang.org
