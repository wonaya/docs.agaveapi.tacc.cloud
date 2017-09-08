# AgaveAPI Docs (Powered by Slate)

This is the working repository for TACC's version of the Agave Science-as-a-Service API.  It uses the [Slate static documentation generator](http://lord.github.io/slate/). 

## Getting started contributing to the Agave API docs

### Prerequisites:

 - Linux or Mac OS X
    - _We don't have enough experience with Docker for Windows to officially support it_
 - Docker CE 17.07+
 - Git 2.12+
 - Proficiency with Markdown

You can develop using a local native Ruby workflow, but that's not supported by our project.

### Quick Set Up

 1. Fork this repository on GitHub
 2. Clone *your forked repository* (not the original one) to your hard drive with `git clone https://github.com/YOURGITHUBUSERNAME/docs.agaveapi.tacc.cloud.git  agave-docs`
 3. `cd agave-docs`
 4. Add a remote branch `git remote add upstream https://github.com/mwvaughn/docs.agaveapi.tacc.cloud.git`
 5. `git checkout -b <new_branch>`
 6. `docker-compose up -d`
 7. View API docs at http://localhost:4567/
 8. Edit away inside `source/`
 9. Commit your changes and merge into `develop`
 10. Issue a PR against the upstream `mwvaughn/agaveapi.docs.tacc.cloud` repository

#### Updating from the upstream repository

Stash or commit your existing work

1. `cd agave-docs`
2. `git pull upstream develop`
3. `git merge develop`

Learn more about [editing Slate markdown](https://github.com/lord/slate/wiki/Markdown-Syntax).
Learn [how to publish your docs](https://github.com/lord/slate/wiki/Deploying-Slate) to GitHub.

### Docker Cheat Sheet

* `docker-compose up -d` launches (or tries to) a doc server on port 4567
* `docker-compose down` will shut down the server
* `docker-compose restart` will, not surprisingly, restart the doc server
* `docker-compose build` will, not surprisingly, restart the doc server
* `docker-compose logs slateapp` will display logs, which can be helpful in debugging rendering issues
* `docker run --rm -v $(pwd):/usr/src/docs -w /usr/src/docs ruby:2.3.1 bundle lock --update` updates local Gemfile.lock

## Need Help? Found a bug?


