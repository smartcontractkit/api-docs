---
title: Oracle Kit Developer Guide

toc_footers:
  - <a href='mailto:support@smartcontract.com'>Need Help?</a>

includes:
  - errors

search: false
---

# Overview

Welcome to the Smart Contract Oracle Kit documentation. Oracle Kit is a set of tools that makes it easy to integrate blockchains with non-blockchain applications. The tools are set up to work well together, but can also be used as standalone tools.

The different parts are:

- [ChainLink](#chainlink): Software for connecting data feeds with the blockchain as needed.
- [WeiWatchers](#weiwatchers): Push notification service for Ethereum based blockchains.
- [Schemas Set](#schema-set): Schemas for defining oracle adapter inputs and outputs.
- [SolC-API](#solc-api): An API for compiling Solidity contracts.

# ChainLink

ChainLink is the core of the oracle kit, coming with built in support for bridging existing websites and APIs with Ethereum and Bitcoin out of the box.

In addition to the [built in](https://chainlink-docs.smartcontract.com/#core-adapters) ChainLink functionality, the oracle can be extended with custom adapters to interact with more specialized serivces and protocols. See the [external adapters](https://chainlink-docs.smartcontract.com/#external-adapters) section for more information on integrating more custom applications.

View [the API documentation](https://smartoracle.smartcontract.com/) and [the source code](https://github.com/oraclekit/chainlink).


# WeiWatchers

WeiWatchers provides push notifications to applications based on Ethereum event logs and account balance changes.

View [the API documentation](https://weiwatchers-docs.smartcontract.com/) and [the source code](https://github.com/oraclekit/wei_watchers).


# Schema Set

The Schema Set allows for pieces of the oracle kit to ensure the data that will be provided from one piece to another will fit what is expected. This allows adapters to reliably be chained together to provide data transformations from sources.

View [the source code](https://github.com/oraclekit/schemas).


# SolC-API

The Solidity Compiler API is a lightweight services wrapping the `solc` Solidity Compiler utility and making it accessible to other web applications via HTTP calls.

View [the source code](https://github.com/oraclekit/solc-api).
