# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout 06bf25c88ecf5d07ad419ef3420448ef75ef7299
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/prod/values.yaml --include-crds
```
