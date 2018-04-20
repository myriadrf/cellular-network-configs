# Osmocom gsm configuration files

## Introduction

Set of configuration files tested working with the osmocom gsm stack and the LimeSDR

## Hardware


* LimeSDR hardware v1.4s, fw=4, hw=4, protocolVersion=1
* Host computer i7-3770 CPU @ 3.40GHz
* Duplexer not tested, band GSM900, arfcn 975,  925.7MHz US ISM/Ham band

## Software 

LimeSuite: git checkout fe53178a<br/>
osmo-trx latest from https://github.com/osmocom/osmo-trx/

### Driver stack

COMPONENT     | DESCRIPTION                      | VERSION  | NOTES     |
--------------|----------------------------------|----------|-----------|
Lime Suite    | LimeSDR driver                   |v17.12.0  |v18 issues |
SoapySDR      | Support library                  |v0.7.0    |           |

### Network stack

COMPONENT     | DESCRIPTION                      | VERSION  | NOTES     |
--------------|----------------------------------|----------|-----------|
osmo-trx      |GSM Radio Modem                   | 0.3.0    |           |

## Configuration

Working config for single host

## Running

Start with osmo-trx -C <config file>    just start in directory with config file osmo-trx.cfg

## Performance

Noticed recent 4/20/2018 improvement in LimeSDR support and gprs stability.

## Changelog

| Version | Date     | Summary
|---------|----------|--------------------
|   0.0   |4/20/2018 | added files        |
|   0.1   |4/20/2018 | update vers        |
