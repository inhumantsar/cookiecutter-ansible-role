# {{cookiecutter.role_name}}

[![Build Status](https://travis-ci.org/{{cookiecutter.author_github}}/ansible-role-{{cookiecutter.role_name}}.svg?branch=master)](https://travis-ci.org/{{cookiecutter.author_github}}/ansible-role-{{cookiecutter.role_name}})

{{cookiecutter.description}}

## Using this Cookiecutter Template
The repo is ready to go for development after answering the cookiecutter questions. There are a few things you will want to tailor before going too far with it:

* Rewrite this README
* [`meta/main.yml`](meta/main.yml): Add Galaxy tags and tailor the supported platforms list. Ensure the copyright information is correct.
* [`.travis.yml`](.travis.yml) and/or [`.gitlab-ci.yml`](.gitlab-ci.yml): Add any additional setup or testing tasks.
* Use [`bumpversion`](https://github.com/peritus/bumpversion) to tag releases and keep your role tidily versioned.

## Requirements

What does the user need to do ahead of time to ensure this role will work for them?

## Supported Platforms

{% if cookiecutter.target_el == 'y' -%}
* RHEL / CentOS: 6, 7
{%- endif %}      
{% if cookiecutter.target_fedora == 'y' -%}
* Fedora: 24-28
{%- endif %}      
{% if cookiecutter.target_debian == 'y' -%}
* Debian:
    - jesse
    - sid
    - stretch
    - buster
{%- endif %}      
{% if cookiecutter.target_ubuntu == 'y' -%}
* Ubuntu
    - bionic
    - artful
    - zesty
    - yakkety
    - xenial
{%- endif %}
{% if cookiecutter.target_alpine == 'y' -%}
* Alpine
{%- endif %}

## Variables & Defaults

Use this space to describe the must-change and should-change variables.

See [`defaults/main.yml`](defaults/main.yml) for more information.

## Usage

Provide an example of the role in action.

## Dependencies

List any other roles which this one depends on and briefly explain why.

## License
[{{cookiecutter.license}}](LICENSE)

## Authors
[{{cookiecutter.author}}](https://github.com/{{cookiecutter.author_github}})