# AgaveAPI Docs (Powered by Slate)

This is the working repository for TACC's version of the Agave Science-as-a-Service API.  It uses the [Slate static documentation generator](http://lord.github.io/slate/). 

## Getting started contributing to the Agave API docs

### Prerequisites:

 - **Linux or Mac OS X**
 - Docker CE 17.07+
 - Git 2.12+
 - Proficiency with Markdown

You can develop using the local Ruby-native workflow, but that's not supported by our project.

### Quick Set Up

 1. Fork this repository on GitHub
 2. Clone *your forked repository* (not the original one) to your hard drive with `git clone https://github.com/YOURUSERNAME/agaveapi.docs.tacc.cloud.git agave-docs`
 3. `cd agave-docs`
 4. `git checkout -b <new_branch>`
 4. `docker-compose -d up`
 5. View API docs at http://localhost:4567/
 6. Edit away inside `source/`
 7. Commit your changes and merge into `develop`
 8. Issue a PR against the upstream `agaveapi.docs.tacc.cloud` repository

Learn more about [editing Slate markdown](https://github.com/lord/slate/wiki/Markdown-Syntax).
Learn [how to publish your docs](https://github.com/lord/slate/wiki/Deploying-Slate) to GitHub.

### Docker Compose Cheat Sheet

* `docker-compose -d up` launches (or tries to) a doc server on port 4567
* `docker-compose down` will shut down the server
* `docker-compose restart` will, not surprisingly, restart the doc server
* `docker-compose logs slateapp` will display logs, which can be helpful in debugging rendering issues

Need Help? Found a bug?
--------------------

