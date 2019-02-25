---
id: us-loader
title: User Stories: Loader
sidebar_label: Loader
---

## Loading data

As a user, I want to see what the structure of the input files are.

- [[VIZ-113](https://shahcompbio.atlassian.net/browse/VIZ-113)] Move/Update parts of main README to docs
- [[VIZ-114](https://shahcompbio.atlassian.net/browse/VIZ-114)] Move/Update loading READMEs to docs

As a user, I want to load tree data as a newick file or gml file.

- [[VIZ-189](https://shahcompbio.atlassian.net/browse/VIZ-189)] Process CorruptTree input prior to loading

As a user, I want to load the outputs of the single cell DNA sequencing pipeline (metrics, segments, bins).

## Interface

As a user, I want an easy way to load the files I need for Lyra into the database, so I don't have to worry about setting up the right systems.

As a user, I want to select files from my computer to open for an analysis, so I don't think about what scripts to run.

- [[VIZ-146](https://shahcompbio.atlassian.net/browse/VIZ-146)] Add input to select from file system instead of drag and drop
- I want to select multiple types, or multiple files for one type
- I want to make sure they're compatible with dashboard (file type, required columns)
- I want to make sure I'm not adding duplicate files
- I want to delete if I add the wrong file

As a user, I want to describe what the metadata of the current analysis is, so I can refer back to it later.

- I need to add a title and brief description
- I want to be able to add other metadata (library, sample) as needed
- Analysis ID should be auto-generated, to prevent collision of IDs.

* [[VIZ-148](https://shahcompbio.atlassian.net/browse/VIZ-148)] Store parsed input files
* [[VIZ-150](https://shahcompbio.atlassian.net/browse/VIZ-150)] Check to see if analysis name already exists

As a user, I want to support the upload of current file types

- Add selecting h5 data (needs to specify key in table)

## Development

As a developer, I want to be able to test the scripts in its current state, to ensure backwards compatibility in the future.

- [[VIZ-115](https://shahcompbio.atlassian.net/browse/VIZ-115)] Create testing framework for python scripts
- [[VIZ-116](https://shahcompbio.atlassian.net/browse/VIZ-116)] Write tests for analysis entry loader
- [[VIZ-117](https://shahcompbio.atlassian.net/browse/VIZ-117)] Write tests for tree loader
- [[VIZ-118](https://shahcompbio.atlassian.net/browse/VIZ-118)] Write tests for segments loader
- [[VIZ-119](https://shahcompbio.atlassian.net/browse/VIZ-119)] Document how to run tests
- [[VIZ-120](https://shahcompbio.atlassian.net/browse/VIZ-120)] Integrate into TravisCI
- [[VIZ-172](https://shahcompbio.atlassian.net/browse/VIZ-172)] Create Docker image for Elasticsearch instance
- [[VIZ-174](https://shahcompbio.atlassian.net/browse/VIZ-174)] Refactor loading scripts

As a developer, I want to be able to modularize the loaders, so I can use them in other projects

- [[VIZ-195](https://shahcompbio.atlassian.net/browse/VIZ-195)] Create package for Python loaders
