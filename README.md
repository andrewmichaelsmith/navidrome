# navidrome

An **experimental** Helm chart for navidrome.

# Quick start

```
help repo add navidrome https://andrewmichaelsmith.github.io/navidrome
helm repo update   
helm install navidrome/navidrome --generate-name
```

# Configuration

Custom values

| Parameter                 | Description | Default |
| ------------------------- | ----------- | ------- |
| persistence.existingClaim | The PVC name that you would like to store music and data. If unset, uses `emptyDir`. | nil |


