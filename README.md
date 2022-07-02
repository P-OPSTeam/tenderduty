# TenderDuty v2

[![Go Reference](https://pkg.go.dev/badge/github.com/blockpane/tenderduty.svg)](https://pkg.go.dev/github.com/blockpane/tenderduty)
[![Gosec](https://github.com/blockpane/tenderduty/workflows/Gosec/badge.svg)](https://github.com/blockpane/tenderduty/actions?query=workflow%3AGosec)
[![CodeQL](https://github.com/blockpane/tenderduty/workflows/CodeQL/badge.svg)](https://github.com/blockpane/tenderduty/actions?query=workflow%3ACodeQL)

Tenderduty is a comprehensive monitoring tool for Tendermint chains. Its primary function is to alert a validator if they are missing blocks, and has many other features.

v2 is complete rewrite of the original tenderduty graciously sponsored by the [Osmosis Grants Program](https://grants.osmosis.zone/). This new version adds a web dashboard, prometheus exporter, telegram and discord notifications, multi-chain support, more granular alerting, and more types of alerts.

![dashboard screenshot](docs/dash.png)

## Documentation

The [documentation](docs/README.md) is a work-in-progress.

## Runtime options:

```
$ tenderduty -h
Usage of tenderduty:
  -example-config
    	print the an example config.yml and exit
  -f string
    	configuration file to use (default "config.yml")
  -state string
    	file for storing state between restarts (default ".tenderduty-state.json")
```

## Installing

Detailed installation info is in the [installation doc.](docs/install.md)

30 second quickstart if you already have Go installed:

```
go install github.com/blockpane/tenderduty@latest
~/go/bin/tenderduty -example-config >config.yml
# edit config
~/go/bin/tenderduty
```
