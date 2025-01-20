# ddev-flysystem-minio: use MinIO for Drupal Flysystem

Configures DGI's Drupal DDEV project to use MinIO for Flysystem storage.

## Installation

```bash
ddev get ddev/ddev-minio
ddev get discoverygarden/ddev-flysystem-minio
ddev restart
```
## Usage

The addon Configures Drupal to use the buckets so no additional configuration is required.

The add depends on [ddev-minio](https://github.com/ddev/ddev-minio/tree/master) to provide minio.
To access the minio console run `ddev minio` and login with `ddevminio` as both the username and password.

### Commands
| Command          | Usage                      | Description                                    |
|------------------|----------------------------|------------------------------------------------|
| `create-buckets` | `ddev create-buckets [-f]` | Creates the flysystem bucket. `-f` to recreate.|

## Uninstall

```bash
ddev get --remove discoverygarden/ddev-flysystem-minio
ddev get --remove ddev/ddev-minio
ddev restart
```
