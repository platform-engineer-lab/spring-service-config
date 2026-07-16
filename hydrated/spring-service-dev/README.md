# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout 0e5419cb16916d636ca85c8ca7e25dbf05148a85
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/dev/values.yaml --include-crds
```
