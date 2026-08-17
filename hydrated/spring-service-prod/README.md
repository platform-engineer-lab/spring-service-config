# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout dbad054a20d772c6bf2bfcea0c80c0a595604880
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/prod/values.yaml --include-crds
```
