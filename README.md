# Factory-X Helm Charts

To have all Factory-X sub-product Helm Charts in one place, a central Factory-X Helm Repository is build. The central Helm Repository is split into two repositories:

- Dev
- Stable

## Helm Repository URL

Both repositories will be hosted via GitHub Pages within this
repository ([factory-x-contributions/charts](https://github.com/factory-x-contributions/charts)) and will be accessible under URL

- [https://factory-x-contributions.github.io/charts/dev](https://factory-x-contributions.github.io/charts/dev) for Dev
- [https://factory-x-contributions.github.io/charts/stable](https://factory-x-contributions.github.io/charts/stable) for Stable

## Availability

### Dev Repository

Dev repository will contain all released Helm Charts of any Factory-X sub-product. Only a certain number of released
Helm charts per Factory-X sub-product might be kept due to clarity reasons.

The Dev Helm repository will be updated once a day.

### Stable repository

Stable repository will contain all Helm charts versions of Factory-X sub-products associated with an official Factory-X
release. Helm charts associated with Factory-X versions which have reached its end of lifetime, will be removed from the stable repository.

The Stable Helm repository will be updated when a new Factory-X release or a patch update is released.

## Usage

### Dev Repository

```shell
$ helm repo add factoryx-dev https://factory-x-contributions.github.io/charts/dev
$ helm search repo factoryx-dev
NAME                                    CHART VERSION   APP VERSION     DESCRIPTION
factoryx-dev/factoryx-connector         0.1.0           0.1.0           A Helm chart for Factory-X Eclipse Data Space C...
factoryx-dev/factoryx-connector-memory  0.1.0           0.1.0           A Helm chart for Factory-X Eclipse Data Space C...

$ helm install factoryx-dev/factoryx-connector
[...]
```
