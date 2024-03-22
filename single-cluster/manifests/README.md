# Manifests Example

This example will deploy the [Kubernetes sample guestbook](https://github.com/kubernetes/examples/tree/master/guestbook/) application.
The app will be deployed into the `mcgonagle-fleet-manifest-example` namespace.

```yaml
kind: GitRepo
apiVersion: fleet.cattle.io/v1alpha1
metadata:
  name: manifests
  namespace: mcgonagle-fleet-manifest-example
spec:
  repo: https://github.com/mcgonagle/fleet-examples
  paths:
    - single-cluster/manifests
```




---
