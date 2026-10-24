# Sphinx Docker Images

This repository containt Docker images used by Mirounga

These images are available at 

- [Docker HUB](https://hub.docker.com/u/mgasphinx)
- [Github Package](https://github.com/orgs/mga-sphinx/packages)

## sphinx-base

![Docker Pulls](https://img.shields.io/docker/pulls/mgasphinx/sphinx)

Python docker image with Sphinx by default

## sphinx-html

![Docker Pulls](https://img.shields.io/docker/pulls/mgasphinx/sphinx-html)

Same as sphinx-base with some additionnals themes

- [furo](https://pradyunsg.me/furo/)
- [sphinx-rtd-theme](https://sphinx-rtd-theme.readthedocs.io/en/stable/) 
- [sphinx-book-theme](https://sphinx-book-theme.readthedocs.io/en/stable/) 
- [sphinx-press-theme](https://schettino72.net/sphinx_press_site/)
- [shibuya](https://shibuya.lepture.com/)

## sphinx-latexpdf

![Docker Pulls](https://img.shields.io/docker/pulls/mgasphinx/sphinx-latexpdf)

Same as sphinx-base, with additonnal LateX packages
to generate a PDF file

## sphinx-ci

![Docker Pulls](https://img.shields.io/docker/pulls/mgasphinx/sphinx-ci)

Same as sphinx-base, with dedicate tools for CI (linter only)
