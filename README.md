# joda.tano.si
[![Homepage][web-img]][web]
[![License][license-img]][license]

This is main Joda web page repository.
Feel free to open a pull request if some content needs updating.


## Prerequisites

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com)
* [Yarn](https://yarnpkg.com)
* [Jekyll](https://jekyllrb.com)


## Installation

* `git clone https://github.com/joda-project/joda.tano.si`
* change into the new directory
* `bundle install`
* `yarn install`


## Running / Development

* `bundle exec jekyll serve`
* visit the page at [http://localhost:4000](http://localhost:4000).

### Deploying

* checkout latest tag/stable code on server
* `bundle install --deployment`
* `bundle exec rake deploy`


[web]: https://joda.tano.si
[license]: https://github.com/joda-project/joda.tano.si/blob/master/LICENSE.md

[web-img]: https://img.shields.io/badge/web-joda.tano.si-green.svg
[license-img]: https://img.shields.io/badge/license-CC%20BY--SA%204.0-blue.svg
