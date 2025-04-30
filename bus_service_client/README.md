# NGTQ Unix Bus Service Client

NGTQ Unix Bus Service Client is a client library for interacting with the NGTQ Unix Bus Service. It provides a simple interface for services to communicate with the message bus through Unix sockets, enabling seamless integration with the NGTQ ecosystem.

## Overview

This client library is an essential component of the NGTQ Unix Bus Service ecosystem, designed to:
- Enable services to communicate with the NGTQ message bus
- Provide a simple, type-safe interface for task queue operations
- Handle serialization and communication through Unix sockets

## Features

- Easy-to-use client interface for bus service communication
- Support for both ID-based and category-based task operations
- Built-in error handling and response management
- Seamless integration with the bus_service_models library

## Installation

Add the following to your Cargo.toml:

```toml
[dependencies]
bus_service_client = "0.1.0"