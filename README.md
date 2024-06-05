# Managed cluster installation

Login to the ACM cluster as cluster admin, then run the following command:

```
helm template . -f values-all.yaml -f values-<environment>.yaml -f values-<cluster name>.yaml | oc apply -f-
```
