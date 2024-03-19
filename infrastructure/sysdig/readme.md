# Sysdig Agent

## Retreiving the Current Helm Chart Version

- `helm repo add sysdig https://charts.sysdig.com`
- `helm repo update`
- `helm search repo sysdig-deploy --versions | head`
- update the version in the `helmrelease.yaml`
