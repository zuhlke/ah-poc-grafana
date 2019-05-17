# ah-poc-grafana

## Run locally

Execute following command to run Grafana on port `8080`
```
./bin/grafana-server web
```

## Deploy To PCF
```
cf push ah-poc-grafana -f manifest.yml
```