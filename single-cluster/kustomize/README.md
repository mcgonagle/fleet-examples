# Kustomize Example

This example will deploy the [Kubernetes sample guestbook](https://github.com/kubernetes/examples/tree/master/guestbook/) application
using kustomize. The app will be deployed into the `fleet-kustomize-example` namespace.

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: kustomize
  namespace: mcgonagle-fleet-kustomize-example
spec:
  repo: https://github.com/mcgonagle/fleet-examples
  paths:
    - single-cluster/kustomize
```
