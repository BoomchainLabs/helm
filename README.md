# Helm

[![Build Status](https://github.com/helm/helm/workflows/release/badge.svg)](https://github.com/helm/helm/actions?workflow=release)
[![Go Report Card](https://goreportcard.com/badge/helm.sh/helm/v4)](https://goreportcard.com/report/helm.sh/helm/v4)
[![GoDoc](https://img.shields.io/static/v1?label=godoc&message=reference&color=blue)](https://pkg.go.dev/helm.sh/helm/v4)
[![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/3131/badge)](https://bestpractices.coreinfrastructure.org/projects/3131)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/helm/helm/badge)](https://scorecard.dev/viewer/?uri=github.com/helm/helm)
[![LFX Health Score](https://insights.production.lfx.dev/api/badge/health-score?project=helm)](https://insights.linuxfoundation.org/project/helm)

Helm is a tool for managing Charts. Charts are packages of pre-configured Kubernetes resources.

Use Helm to:

- Find and use [popular software packaged as Helm Charts](https://artifacthub.io/packages/search?kind=0) to run in Kubernetes
- Share your own applications as Helm Charts
- Create reproducible builds of your Kubernetes applications
- Intelligently manage your Kubernetes manifest files
- Manage releases of Helm packages

## Helm in a Handbasket

Helm is a tool that streamlines installing and managing Kubernetes applications.
Think of it like apt/yum/homebrew for Kubernetes.

- Helm renders your templates and communicates with the Kubernetes API
- Helm runs on your laptop, CI/CD, or wherever you want it to run.
- Charts are Helm packages that contain at least two things:
  - A description of the package (`Chart.yaml`)
  - One or more templates, which contain Kubernetes manifest files
- Charts can be stored on disk, or fetched from remote chart repositories
  (like Debian or RedHat packages)

## Helm Development and Stable Versions

Helm v4 is currently under development on the `main` branch. This is unstable and the APIs within the Go SDK and at the command line are changing.
Helm v3 (current stable) is maintained on the `dev-v3` branch. APIs there follow semantic versioning.

## Install

Binary downloads of the Helm client can be found on [the Releases page](https://github.com/helm/helm/releases/latest).

Unpack the `helm` binary and add it to your PATH and you are good to go!

If you want to use a package manager:

- [Homebrew](https://brew.sh/) users can use `brew install helm`.
- [Chocolatey](https://chocolatey.org/) users can use `choco install kubernetes-helm`.
- [Winget](https://learn.microsoft.com/en-us/windows/package-manager/) users can use `winget install Helm.Helm`.
- [Scoop](https://scoop.sh/) users can use `scoop install helm`.
- [Snapcraft](https://snapcraft.io/) users can use `snap install helm --classic`.
- [Flox](https://flox.dev) users can use `flox install kubernetes-helm`.

To rapidly get Helm up and running, start with the [Quick Start Guide](https://helm.sh/docs/intro/quickstart/).

See the [installation guide](https://helm.sh/docs/intro/install/) for more options,
including installing pre-releases.

## Docs

Get started with the [Quick Start guide](https://helm.sh/docs/intro/quickstart/) or plunge into the [complete documentation](https://helm.sh/docs).

## Roadmap

The [Helm roadmap uses GitHub milestones](https://github.com/helm/helm/milestones) to track the progress of the project.

The development of Helm v4 is currently happening on the `main` branch while the development of Helm v3, the stable branch, is happening on the `dev-v3` branch. Changes should be made to the `main` branch prior to being added to the `dev-v3` branch so that all changes are carried along to Helm v4.

## Community, discussion, contribution, and support

You can reach the Helm community and developers via the following channels:

- [Kubernetes Slack](https://kubernetes.slack.com):
  - [#helm-users](https://kubernetes.slack.com/messages/helm-users)
  - [#helm-dev](https://kubernetes.slack.com/messages/helm-dev)
  - [#charts](https://kubernetes.slack.com/messages/charts)
- Mailing List:
  - [Helm Mailing List](https://lists.cncf.io/g/cncf-helm)
- Developer Call: Thursdays at 9:30-10:00 Pacific ([meeting details](https://github.com/helm/community/blob/master/communication.md#meetings))

### Contribution

If you're interested in contributing, please refer to the [Contributing Guide](CONTRIBUTING.md) **before submitting a pull request**.

### Code of conduct

Participation in the Helm community is governed by the [Code of Conduct](code-of-conduct.md).
