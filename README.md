# NGTQ Unix Bus Service

NGTQ Unix Bus Service is a message bus implementation built on top of the NGTQ and NGTask_Queue_Basic crates. It provides a Unix socket-based communication layer for task queue operations, enabling seamless integration of NGTQ in Linux environments.

## Overview

This project is part of the NGTQ ecosystem and consists of several components:

- **ngtq_unix_bus_service**: The main bus service that use NGTask_Queue_Basic as the NGTQ implementation for its domain
- **bus_service_models**: A shared library containing data models used by both the service and client.
- **integration_tests**: A test suite to ensure proper functionality of the entire system.

## Features

- Unix socket-based communication for inter-process task queue operations
- Support for both ID-based and category-based tasks
- Configurable socket path via command-line arguments, config file, or default value
- Comprehensive integration tests

## Installation

Add the following to your Cargo.toml:

```toml
[dependencies]
ngtq = "0.1.0"
ngtask_queue_basic = "0.1.0"
```

Using the Client-side Library
rust
Copy

// coming soon

Configuration

The socket path can be configured in three ways (in order of precedence):

    Command-line argument: --socket-path /path/to/socket
    Configuration file: ngtq_unix_bus_service_config.json
    Default value: /tmp/resu_ipc_socket

Related Projects

    NGTQ: The core trait definition for Next Generation Task Queues
    NGTask_Queue_Basic: A basic implementation of the NGTQ trait

Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
License

This project is licensed under the MIT License - see the LICENSE file for details.