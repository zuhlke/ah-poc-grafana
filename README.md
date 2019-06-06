# ah-poc-grafana

[![Build Status](https://travis-ci.org/zuhlke/ah-poc-grafana.svg?branch=master)](https://travis-ci.org/zuhlke/ah-poc-grafana)

## Run locally

Execute following command to run Grafana on port `8080`

`./bin/grafana-server web`

## Deploy To PCF

Automatically deployed via Travis on each commit or manually by`cf push`

## Setup

Our default datasource and dashboard are configured automatically. These are loaded on startup.

Grafana is configured by files in the `conf/` folder. The top-level config is `defaults.ini`. As the name suggests, this is the default config.

The provisioning directory contains the datasource and dashboards config files. The provisioning directory
is defined within `defaults.ini`, and is `conf/provisioning/`.

In the `datasources/` and `dashboards/` subfolders, yaml files configure the respective components of Grafana.

## Updating the configuration

If you update the configuration in this repo and then push your changes to GitHub, Travis will redeploy the app and Grafana will restart and pick up the configuration changes.
