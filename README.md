# Meiliadmin

[Meiliadmin](https://kaermorchen.github.io/meiliadmin/) is an admin panel for [Meilisearch](https://www.meilisearch.com/).

## Prerequisites

You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/) (with npm)
* [Ember CLI](https://cli.emberjs.com/release/)
* [Google Chrome](https://google.com/chrome/)

## Installation

* `git clone <repository-url>` this repository
* `cd meiliadmin`
* `npm install`

## Running / Development

* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).
* Visit your tests at [http://localhost:4200/tests](http://localhost:4200/tests).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

* `ember test`
* `ember test --server`

### Linting

* `npm run lint`
* `npm run lint:fix`

### Building

* `ember build` (development)
* `ember build --environment production` (production)

## Further Reading / Useful Links

* [ember.js](https://emberjs.com/)
* [ember-cli](https://cli.emberjs.com/release/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)

## Install Meilisearch
```bash
# Create folder
$ mkdir data && cd data

# Install Meilisearch
$ curl -L https://install.meilisearch.com | sh

# Download a dataset
$ curl https://docs.meilisearch.com/meteorites.json --output meteorites.json

# Start Meilisearch
$ ./meilisearch

# Create a new index `meteorites` and push the dataset
$ curl -X POST 'http://localhost:7700/indexes/meteorites/documents' -H 'Content-Type: application/json' --data-binary @meteorites.json
```
