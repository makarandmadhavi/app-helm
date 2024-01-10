# k8s Infrastructure

## Deploy database

```helm install my-release oci://registry-1.docker.io/bitnamicharts/mariadb```

## Deploy REST API webapp

1. ``` kubectl create namespace app ```
2. ``` helm upgrade --install webapp ./ -n app ```

## Running Jmeter test
```
jmeter -n -t /Users/makarandmadhavi/Desktop/NEU/Cloud/infra/iac-pulumi/jmeter-test.jmx -l results/test_results.jtl -e -o results/dashboard

```