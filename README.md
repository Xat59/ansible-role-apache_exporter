# ansible-role-apache_exporter

[![Build Status](https://api.travis-ci.com/Xat59/ansible-role-apache_exporter.svg?branch=master)](https://travis-ci.com/github/Xat59/ansible-role-apache_exporter)

This ansible role installs a Prometheus Apache Exporter.

- [Getting Started](#getting-started)
  - [Prerequisities](#prerequisities)
  - [Installing](#installing)
- [Usage](#usage)
- [Testing](#testing)
- [Built With](#built-with)
- [Versioning](#versioning)
- [Authors](#authors)
- [License](#license)
- [Contributing](#contributing)

## Getting Started

These instructions will get you a copy of the role for your ansible playbook. Once launched, it will install an [Prometheus Apache Exporter](https://github.com/Lusitaniae/apache_exporter) server.

### Prerequisities

Ansible 2.10.x version installed.

### Installing

Create or add to your roles dependency file (e.g requirements.yml):

```yaml
- src: xat.apache_exporter
  version: 2.0.0
  name: apache_exporter
```

Install the role with ansible-galaxy command:

`ansible-galaxy install -p roles -r requirements.yml -f`

Use in a playbook:

```yaml
---
- hosts: someserver
  roles:
    - role: apache_exporter
```

## Usage

Look to the [defaults](defaults/main.yml) properties file to see the possible configuration properties. To work properly apache module `mod_status` should be enabled and configure.

## Testing

`molecule test`

## Built With

![Ansible](https://img.shields.io/badge/ansible-2.10.x-green.svg)
![Molecule](https://img.shields.io/badge/molecule-3.3.0-green.svg)

## Versioning

For the versions available, see the [tags on this repository](https://github.com/Xat59/ansible-role-apache_exporter/tags).

Additionaly you can see what change in each version in the [CHANGELOG.md](CHANGELOG.md) file.

## Authors

- this repo is now maintained by **xat** - [xat](https://github.com/Xat59)
- initialy forked from **Idealista** - [idealista](https://github.com/idealista)

## License

![Apache 2.0 Licence](https://img.shields.io/hexpm/l/plug.svg)

This project is licensed under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license - see the [LICENSE.txt](LICENSE.txt) file for details.

## Contributing

Please read [CONTRIBUTING.md](.github/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
