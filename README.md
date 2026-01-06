# Keycloak-chart

This keycloak-chart installs keycloak:17.0.0. To install the latest version of chart we can use latest keycloak chart available on web. 
## Installation.


``` shell
helm install keycloak . -n keycloak --create-namespace
```

  To install the chart in an existing namespace, use the following command:

``` shell

helm install keycloak. -n keycloak
```

 To uninstall the chart, execute the following command:


``` shell
helm uninstall keycloak -n keycloak

```


## Theme Structure

This repository contains a custom Keycloak theme with:
- login
- account
- admin (optional)

The theme follows standard Keycloak directory conventions.

## Ingress & TLS Configuration

The Helm chart supports configuring TLS via cert-manager.

Recommended setup:
- Production: letsencrypt-prod
- Non-production: letsencrypt-staging

The clusterIssuer can be overridden using Vvalues.yaml per environment.
