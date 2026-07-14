# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout ed4cd024d4116a70ea1b9bd95991239eaa2abee6
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/dev/values.yaml --include-crds
```
