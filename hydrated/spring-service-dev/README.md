# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout 668cc4d5e107d53be20f939827f4119f95cc3e43
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/dev/values.yaml --include-crds
```
