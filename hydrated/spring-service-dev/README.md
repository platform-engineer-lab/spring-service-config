# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout b041cbcad5998b53544868aa8fe4c9587f61ff0d
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/dev/values.yaml --include-crds
```
