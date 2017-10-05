[![buildstatus](https://travis-ci.org/culshoefer/pyarxiv.svg?branch=master)](https://travis-ci.org/culshoefer/pyarxiv)[![Coverage Status](https://coveralls.io/repos/github/culshoefer/pyarxiv/badge.svg?branch=master)](https://coveralls.io/github/culshoefer/pyarxiv?branch=master)
# pyarxiv

pyarxiv is a wrapper for the API of [Cornell University's famous repository](http://arxiv.org) for scientific papers and the like.


## Installation
TODO

## Features
- Query the arXiv API (atom feed) in your code
- Use enums for arXiv categories
- Download papers in your code as PDF
TODO - Do the above in the commandline

## Usage

### CLI
```sh
# will download a couple of papers with given ids to folder /home/user, name them according to their titles,
# append their arxiv ids, and do not give progress feedback when each paper is downloaded
pyarxiv-cli download 1703.00001 1703.00002v1 ... --target-folder=/home/user --use-title-for-filename --append-id --silent
# Queries for papers with "Lorem" in them, maximally gets 5 papers (default 100), authors Einstein and Zweistein
# Other potential arguments are --abstract, --journalref and manualmode with --querystring
pyarxiv-cli query --title="Lorem" --max-results=5 --authors="A Einstein, B Zweistein"
```

### Python

TODO
