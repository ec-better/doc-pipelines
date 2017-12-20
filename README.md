## Pipelines documentation

[![Build Status](https://build.terradue.com/buildStatus/icon?job=doc-t2-api)](https://build.terradue.com/job/doc-t2-api/)

This is the official repository of the pipelines documentation

This documentation is live at: http://docs.terradue.com/pipelines/

### Getting started

Here's the procedure to install the required packages

1) Install sphinx

```bash
sudo conda install sphinx
sudo conda install sphinx_bootstrap_theme
sudo conda install sphinx_rtd_theme
sudo conda install sphinxcontrib-plantuml
```

2) If needed, set your github information:

```bash
$ git config --global user.name <github username>
$ git config --global user.email <email address>
```

### Building locally

Build the documentation by running ``make html`` or ``make latex``

### Continuous build

The PDF is generated at http://docs.terradue.com/pipelines/pipelines.pdf every time a change is pushed on the repo.

#### This documentation is built with [sphinx](http://sphinx-doc.org/).
