## WarpStream Self-Hosted Control Plane Helm Chart

This repository contains the Helm chart for the WarpStream self-hosted control plane
and automatically publishes it to the Helm repo, located at [warpstreamlabs.github.io/shcp](https://warpstreamlabs.github.io/shcp).
See the [chart README](charts/warpstream-self-hosted-control-plane/README.md) for installation instructions.

The WarpStream agent chart lives in [warpstreamlabs/charts](https://github.com/warpstreamlabs/charts).

This project relies on [chart-releaser Action](https://github.com/helm/chart-releaser-action)
to package/update/publish Helm charts. When new commits are pushed on `main`,
[Chart Releaser](https://github.com/helm/chart-releaser) scans folders under `charts/`
for new versions and creates the corresponding GitHub Releases.

For publishing a new Chart release, push a commit incrementing `version` in `Chart.yaml`.
