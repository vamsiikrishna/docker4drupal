# Docker-based Drupal environment for local development

[![Documentation Status](https://readthedocs.org/projects/docker4drupal/badge/?version=latest)](http://docs.docker4drupal.org)
[![Build Status](https://travis-ci.org/wodby/docker4drupal.svg?branch=master)](https://travis-ci.org/wodby/docker4drupal)

[![Wodby Slack](https://www.google.com/s2/favicons?domain=www.slack.com) Join us on Slack](https://slack.wodby.com/)

## Introduction

Docker4Drupal is a set of docker images optimized for local development with Drupal. Use docker-compose.yml file from this repository to spin up local environment on Linux, Mac OS X and Windows. 

Read [**Getting Started**](http://docs.docker4drupal.org/en/latest/).

## Bundle

The Drupal bundle consist of the following containers:

| Container | Versions | Service name | Image | Enabled by default |
| --------- | -------- | ------------ | ----- | ------------------ |
| Nginx      | 1.10               | nginx     | [wodby/drupal-nginx](https://github.com/wodby/drupal-nginx/)            | ✓ |
| PHP        | 5.3, 5.6, 7.0, 7.1 | php       | [wodby/drupal-php](https://github.com/wodby/drupal-php/)                | ✓ |
| MariaDB    | 10.1               | mariadb   | [wodby/mariadb](https://github.com/wodby/mariadb/)                      | ✓ |
| Redis      | 3.2                | redis     | [wodby/redis](https://github.com/wodby/redis/)                          | ✓ |
| Varnish    | 4.1                | varnish   | [wodby/drupal-varnish](https://github.com/wodby/drupal-varnish)         |   |
| Solr       | 5.5, 6.3, 6.4      | solr      | [wodby/drupal-solr](https://github.com/wodby/drupal-solr)               |   |
| phpMyAdmin | latest             | pma       | [phpmyadmin/phpmyadmin](https://hub.docker.com/r/phpmyadmin/phpmyadmin) | ✓ |
| Mailhog    | latest             | mailhog   | [mailhog/mailhog](https://hub.docker.com/r/mailhog/mailhog)             | ✓ |
| Node.js    | 7                  | node      | [_/node](https://hub.docker.com/_/node)                                 |   |
| Memcached  | latest             | memcached | [_/memcached](https://hub.docker.com/_/memcached/)                      |   |
| Traefik    | latest             | traefik   | [_/traefik](https://hub.docker.com/_/traefik/)                          |   |

Supported Drupal versions: 6, 7, 8.

## Documentation

Full documentation is available at http://docs.docker4drupal.org/.

## Using in Production

Deploy docker-based infrastructure for Drupal to your own server via [![Wodby](https://www.google.com/s2/favicons?domain=wodby.com) Wodby](https://wodby.com).

## License

This project is licensed under the MIT open source license.
