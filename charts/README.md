# Smoketest


helm upgrade \
  --create-namespace \
  --install \
  --wait \
  --namespace=open5gs \
  "pcf" \
  "$(git rev-parse --show-toplevel)/charts/pcf"