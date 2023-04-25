## Usage

```
# to build a new helm charts package (tarball)
$ helm package charts/rudderstack-helm/
$ mv rudderstack-<version>.tgz docs

# add to the index
$ helm repo index docs --url https://luxorlabs.github.io/helm-charts

# add the repo if it is not added yet
$ helm repo add luxor-helm https://luxorlabs.github.io/helm-charts/

# pull helm repo update
$ helm repo update

# check the desired version exists
$ helm search repo rudder -l
```