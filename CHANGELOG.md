# Changelog

## 1.1.2

- Fixed increasing memory consumption (#78)

## 1.1.1

- Fixed an error in "skip tables" functionality (#73)

## 1.1.0

- Changed config file format from INI to YAML
- Support for UUID, decimal, numeric, char(N) and character(N) data types
- Support for multiple schemas synchronization
- Excluding tables from synchronization

## 1.0.7

- Updated public server URL (#63)
- Updated to mergin-client 0.7.3

## 1.0.6

- Updated to geodiff 1.0.4 and mergin-client 0.6.5 (#50)

## 1.0.5

- Switched to geodiff 1.0 and mergin-client 0.6 (#49)
- Robustness improvement: mark base schema as invalid if init fails (#46)

## 1.0.4

- More fixes for loss of precision of floating point numbers
- Fixed support for character varying(X) data type (#44)

## 1.0.3

- Fixed loss of precision of floating point numbers (geodiff #110)
- Fixed writing of "empty" flag of geometries (geodiff #112)
- Support for more PostgreSQL data types - bigint, smallint, character varying (#41, geodiff #111)
- Fixed initialization from database (#42)

## 1.0.2

- Fixed two bugs related to copying of data between GPKG and PostgreSQL (geodiff #108, #109)
- Added an extra check during the init to verify data got copied correctly (#37)
- Added display of mergin-db-sync version when the daemon starts

## 1.0.1
 -  Fixed handling of local working directory in init function

## 1.0  (2021/03/25)

The first official release of mergin-db-sync! It includes all the essential functionality to set up and maintain
sync between a Mergin project and a PostgreSQL database.

The tool can be run from CLI on demand with low-level commands (init, pull, push) or it can be started as a daemon
to continuously maintain data in sync. It can be also run using a Docker container: lutraconsulting/mergin-db-sync
