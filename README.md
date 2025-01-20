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



