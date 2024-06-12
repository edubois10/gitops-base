helm dependency build

helm upgrade -i sealed-secrets . --create-namespace --namespace sealed-secrets

sseal < secret.yaml > sssealed-secret.yaml