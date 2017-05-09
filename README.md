# inline-precompile-error

This is a minimal reproduction of the error:
```
Uncaught Error:
Error: Could not find module `htmlbars-inline-precompile` imported from `dummy/tests/integration/components/thing-1-test` at http://localhost:7357/assets/test-support.
js, line 6993
```

## Installation

* `git clone <repository-url>` this repository
* `cd inline-precompile-error`
* `yarn install`

## Running Tests

* `ember test --server`

## Notes

The error appears to be caused by [ember-cli-stylelint](https://github.com/billybonks/ember-cli-stylelint).
If you run `yarn remove ember-cli-stylelint` and re-run the tests, they pass.
