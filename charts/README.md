# Smoketest


helm upgrade \
  --create-namespace \
  --install \
  --wait \
  --namespace=open5gs \
  "udr" \
  "$(git rev-parse --show-toplevel)/charts/udr"