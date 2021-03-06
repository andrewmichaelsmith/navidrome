# Navidrome

An **experimental** Helm chart for [Navidrome](https://www.navidrome.org/).

# Quick start

```
helm repo add navidrome https://andrewmichaelsmith.github.io/navidrome
helm repo update
helm install navidrome/navidrome --generate-name
```

# Configuration

Custom values

| Parameter                 | Description | Default |
| ------------------------- | ----------- | ------- |
| persistence.enabled| Whether to use persistence for music and data. If unset, uses `emptyDir`. | false |
| persistence.existingClaim | If using persistence, the PVC name that you would like to store music and data. | nil |



# Release flow

- Update `Chart.yaml` and `values.yaml`
- Merge/commit to main
- "Draft new release" on github (create new tag)
- Wait for github-pages update
- `helm upgrade navidrome-<id> navidrome/navidrome`
