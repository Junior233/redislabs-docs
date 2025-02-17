---
Title: redis-di delete
linkTitle: redis-di delete
description: Delete RDI database permanently
weight: 10
alwaysopen: false
categories: ["redis-di"]
aliases: 
---

Delete RDI database permanently

## Usage

```
Usage: redis-di delete [OPTIONS]
```

## Options
* `loglevel`: 
  * Type: Choice(['DEBUG', 'INFO', 'WARN', 'ERROR', 'CRITICAL']) 
  * Default: `info`
  * Usage: `--loglevel
-log-level`

  


* `cluster_host` (REQUIRED): 
  * Type: STRING 
  * Default: `none`
  * Usage: `--cluster-host`

  Host/IP of Redis Enterprise Cluster (service name in case of k8s)


* `cluster_api_port` (REQUIRED): 
  * Type: INT 
  * Default: `9443`
  * Usage: `--cluster-api-port`

  API Port of Redis Enterprise Cluster


* `cluster_user` (REQUIRED): 
  * Type: STRING 
  * Default: `none`
  * Usage: `--cluster-user`

  Redis Enterprise Cluster username with either DB Member, Cluster Member or Cluster Admin roles


* `cluster_password`: 
  * Type: STRING 
  * Default: `none`
  * Usage: `--cluster-password`

  Redis Enterprise Cluster Password


* `rdi_host` (REQUIRED): 
  * Type: STRING 
  * Default: `none`
  * Usage: `--rdi-host`

  Host/IP of RDI Database


* `rdi_port` (REQUIRED): 
  * Type: INT 
  * Default: `none`
  * Usage: `--rdi-port`

  Port of RDI Database


* `rdi_password`: 
  * Type: STRING 
  * Default: `none`
  * Usage: `--rdi-password`

  RDI Database Password


* `rdi_key`: 
  * Type: STRING 
  * Default: `none`
  * Usage: `--rdi-key`

  Private key file to authenticate with


* `rdi_cert`: 
  * Type: STRING 
  * Default: `none`
  * Usage: `--rdi-cert`

  Client certificate file to authenticate with


* `rdi_cacert`: 
  * Type: STRING 
  * Default: `none`
  * Usage: `--rdi-cacert`

  CA certificate file to verify with


* `force`: 
  * Type: BOOL 
  * Default: `false`
  * Usage: `--force
-f`

  Force operation. skips verification prompts


* `help`: 
  * Type: BOOL 
  * Default: `false`
  * Usage: `--help`

  Show this message and exit.



## CLI Help

```
Usage: redis-di delete [OPTIONS]

  Deletes RDI database permanently

Options:
  -log-level, --loglevel [DEBUG|INFO|WARN|ERROR|CRITICAL]
                                  [default: INFO]
  --cluster-host TEXT             Host/IP of Redis Enterprise Cluster (service
                                  name in case of k8s)  [required]
  --cluster-api-port INTEGER      API Port of Redis Enterprise Cluster
                                  [default: 9443; required]
  --cluster-user TEXT             Redis Enterprise Cluster username with
                                  either DB Member, Cluster Member or Cluster
                                  Admin roles  [required]
  --cluster-password TEXT         Redis Enterprise Cluster Password
  --rdi-host TEXT                 Host/IP of RDI Database  [required]
  --rdi-port INTEGER              Port of RDI Database  [required]
  --rdi-password TEXT             RDI Database Password
  --rdi-key TEXT                  Private key file to authenticate with
  --rdi-cert TEXT                 Client certificate file to authenticate with
  --rdi-cacert TEXT               CA certificate file to verify with
  -f, --force                     Force operation. skips verification prompts
  --help                          Show this message and exit.
```

