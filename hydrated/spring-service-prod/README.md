# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout 69d0900f13a29f62b6d0a5d10f9a0eeb4f70b5fe
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/prod/values.yaml --include-crds
```
