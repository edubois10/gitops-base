To reset the argocd user password:
1. Modify the admin.password of the $ARGOCD_CR_NAME-cluster secret
2. oc -n openshift-gitops patch secret argocd-secret --patch "{\"data\": {\"admin.password\": null}}"
secret/argocd-secret patched