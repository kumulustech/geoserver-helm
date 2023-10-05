# A Kubernetes HELM Chart for the Geoserver monolith application

Based on, and extending the work done in dockerizing geoserver: [geoserver-docker](https://github.com/geoserver/docker)

## Install this chart

You likely want to make at least a minimum configuration values.yaml with at least something like the following:


```yaml
persistence:
  enabled: true
  size: 50Gi
```

Clone this repository to a machine with the helm binary from [helm.sh](https://helm.sh), review the default values, and install.

```
helm install geoserver geoserver --repo https://kumulustech.github.io/geoserver-helm --values values.yaml
```

## Contributing

Fork and submit a pull request.  We follow the code of conduct outlined in our [Code of Conduct](CODEOFCONDUCT.md) file in the root directory of the repository.
