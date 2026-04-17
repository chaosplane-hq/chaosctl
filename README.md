# chaosctl
CLI for [ChaosPlane](https://chaosplane.io) — chaos engineering platform for Kubernetes.

## Install

### macOS (Homebrew)

```bash
brew install chaosplane-hq/tap/chaosctl
```

### Linux / macOS (manual)

```bash
curl -fsSL https://github.com/chaosplane-hq/chaosctl/releases/latest/download/chaosctl_$(uname -s | tr '[:upper:]' '[:lower:]')_$(uname -m | sed 's/x86_64/amd64/;s/aarch64/arm64/').tar.gz | tar xz
sudo mv chaosctl /usr/local/bin/
```

### Verify

```bash
chaosctl version
```

## Usage

```bash
chaosctl experiment create -f experiment.yaml
chaosctl experiment list
chaosctl experiment status my-experiment
chaosctl experiment abort my-experiment
```

## License
Apache License 2.0
