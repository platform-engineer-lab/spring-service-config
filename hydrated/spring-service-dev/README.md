# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/platform-engineer-lab/spring-service-config
# cd into the cloned directory
git checkout 2300f0ff77ad1111056eb019aa780c811068940c
helm template . --name-template spring-service --namespace business-apps --values ./chart/env/dev/values.yaml --include-crds
```
