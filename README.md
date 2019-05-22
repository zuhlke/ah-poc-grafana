# ah-poc-grafana

## Run locally

Execute following command to run Grafana on port `8080`

`./bin/grafana-server web`

## Deploy To PCF

`cf push`

## Importing the dashboard

When you're in the GUI, to import the dashboard created by Jason from a public template, go to the left side 
of the GUI:

1. Big '+' button
2. Import
3. Upload json file
4. Choose the file ah-poc-grafana-configuration.json which is in `conf/provisioning/dashboards/json-dashboards` from this repo.
5. Save with the default settings
6. Tada!
