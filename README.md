# HelloID-Conn-Prov-HR-Generator
Template repository for HelloID Provisioning Target Connector

<a href="https://github.com/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator/network/members"><img src="https://img.shields.io/github/forks/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator" alt="Forks Badge"/></a>
<a href="https://github.com/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator/pulls"><img src="https://img.shields.io/github/issues-pr/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator" alt="Pull Requests Badge"/></a>
<a href="https://github.com/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator/issues"><img src="https://img.shields.io/github/issues/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator" alt="Issues Badge"/></a>
<a href="https://github.com/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/Tools4everBV/HelloID-Conn-Prov-Source-HR-Generator?color=2b9348"></a>

| :warning: Warning                                                                         |
| :---------------------------------------------------------------------------------------- |
| This is a demo repository that creates random person data. |

| :information_source: Information                                                         |
| :--------------------------------------------------------------------------------------- |
|   This system automatically generate persons using HR generator library |

## Versioning
| Version | Description     |
| ------- | --------------- |
| v1.0.0-alpha   | Initial release |

<!-- TABLE OF CONTENTS -->
## Table of Contents
- [HelloID-Conn-Prov-Target-Template](#helloid-conn-prov-HR-Generator)
  - [Versioning](#versioning)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [Getting Started](#getting-started)
  - [Getting help](#getting-help)
  - [HelloID Docs](#helloid-docs)

## Introduction

This system automatically generate persons using HR generator library.

| Action | Action(s) Performed | Comment |
| ------ | ------------------- | ------- |
| person.ps1                | create persons                                             |    |
| department.ps1            | create department                                          |    |

## Getting Started

HR generator source systems are configured similarly to standard Source systems, but in place of a Persons import script and Departments import script, they have the following settings, located on the Configuration tab.

| Setting | Description | Mandatory |
| ------- | ----------- | --------- |
| Number Of Persons To Generate                | The number of employees generated for the system's raw personnel data, which become Persons during the import process.                                             | Yes   |
| Seed            | An integer that determines the RNG seed used to generate the example data. Typically only needs to be changed if you have multiple HR generator systems, and you want them to have different data. | Yes   |
| Number Of Contracts To Generate Per Person            | The number of Contracts to generate for each person. | Yes   |
| Display Name Convention            | Change how persons' Display names are formatted. | Yes   |
| Contract Calculation            |  | Yes   |
| Percentage Of Persons With Inactive Contracts            | Percentage of persons with only Inactive contracts. | Yes   |
| Number Of Departments To Generate            | The number of Departments to generate. | Yes   |
| Percentage Of Departments With A Parent Department            | The percentage of Departments with a ParentExternalId defined. See Departments import script. | Yes   |

## Getting help
> _For more information on how to configure a HelloID PowerShell connector, please refer to our [documentation](https://docs.helloid.com/en/provisioning/source-systems.html) pages_

## HelloID Docs
The official HelloID documentation can be found at: https://docs.helloid.com/
