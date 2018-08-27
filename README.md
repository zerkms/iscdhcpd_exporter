# ISC-DHCPD exporter

[![CircleCI](https://circleci.com/gh/spagno/iscdhcpd_exporter/tree/master.svg?style=shield)][circleci]
[![Docker Pulls](https://img.shields.io/docker/pulls/spagno/iscdhcpd-exporter.svg?maxAge=604800)][hub]
[![Go Report Card](https://goreportcard.com/badge/github.com/spagno/iscdhcpd_exporter)][goreportcard]

Prometheus exporter for isc dhcpd server exposed by \*NIX systems, written
in Go.

## Building and running

Prerequisites:

* [Go compiler](https://golang.org/dl/)
* dhcpd-pools installed on the target server

Building:

    go get github.com/spagno/iscdhcpd_exporter
    cd ${GOPATH-$HOME/go}/src/github.com/spagno/iscdhcpd_exporter
    make
    ./iscdhcpd_exporter <flags>

To see all available configuration flags:

    ./iscdhcpd_exporter -h
