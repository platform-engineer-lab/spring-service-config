# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout 2683b9b1e10ed73090e82b7625e3979f1c677b30
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/prod/values.yaml --include-crds
```
