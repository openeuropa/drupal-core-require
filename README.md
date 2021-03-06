# drupal-core-require

[![Build Status](https://drone.fpfis.eu/api/badges/openeuropa/drupal-core-require/status.svg?branch=8.6.x)](https://drone.fpfis.eu/openeuropa/drupal-core-require)
[![Packagist](https://img.shields.io/packagist/v/openeuropa/drupal-core-require.svg)](https://packagist.org/packages/openeuropa/drupal-core-require)

``openeuropa/drupal-core-require`` provides the ``require`` dependencies of ``drupal/core`` as a standalone package.
It follows the same release cycle and versioning scheme as Drupal core.
You should use the same version constraint for it as you use for Drupal core.

It applies some patches on ``drupal/core`` that are needed in OPENEUROPA modules.

## Patches list

- [Patch](https://www.drupal.org/files/issues/2018-09-14/2189267-88.patch) for Core issue [#2189267](https://www.drupal.org/project/drupal/issues/2189267) -
When content language detection is different from interface language detection, the detected language must be applied to the rendered content.

## Usage

### Drupal Core 8.6.x

``composer require openeuropa/drupal-core-require ^8.6``

## Installation using Docker Compose

The setup procedure can be simplified by using Docker Compose.

Requirements:

- [Docker](https://www.docker.com/get-docker)
- [Docker-compose](https://docs.docker.com/compose/)

Run:

```bash
docker-compose up -d
```

Then:

```bash
$ docker-compose exec web composer install
```
