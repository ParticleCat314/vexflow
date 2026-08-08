# Development Guide

This guide collects the build and test instructions that were previously spread across the repository.

## Setup

From the repository root:

```sh
npm install
```

## Common Commands

- `grunt` — build the complete set of VexFlow libraries
- `npm run lint` — run ESLint
- `npm test` — build the debug libraries and run the QUnit command line tests
- `grunt build:docs` — generate the API reference into `docs/api/`

## Development Workflows

- `grunt watch` — fastest debug CJS rebuild loop
- `grunt webpack:watchDebug` — watch debug builds without cleaning `build/`
- `grunt watch:esm` — watch and build ESM output
- `grunt watch:prod` — watch and build production bundles

## Test Workflows

- `grunt test:cmd` — run the QUnit command line tests
- `grunt test:browser:cjs` — open the browser test page using the CJS build
- `grunt test:browser:esm` — serve the repository locally and open the browser test page using the ESM build

## Reference / Visual Regression Workflows

- `grunt reference` — build the current revision and copy it to `reference/`
- `grunt generate:current` — create images from the current build
- `grunt generate:reference` — create images from the reference build
- `grunt test:reference` — compare generated images from current and reference builds
- `grunt test:reference:cache` — reuse existing reference images when available

## Demos

See [../demos/README.md](../demos/README.md) for demo-specific instructions and links to each demo area.
