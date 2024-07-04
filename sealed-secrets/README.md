## Steps

1. Deploy with helm the sealed-secrets
   1. helm dependency build

   2. helm upgrade -i sealed-secrets . --create-namespace --namespace sealed-secrets

   3. sseal < secret.yaml > sssealed-secret.yaml
2. Install the operator from the operator hub and create the argcd application from the repo.