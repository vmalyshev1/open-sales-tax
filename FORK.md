# About this fork

`vmalyshev1/open-sales-tax` is a fork of
[ejosterberg/open-sales-tax](https://github.com/ejosterberg/open-sales-tax)
(OpenSalesTax, Apache License 2.0). It serves as the rates engine for the
private US-Sales-Tax-Calc app.

The upstream `LICENSE` and `NOTICE` files and all upstream copyright headers
are kept unchanged. Files changed in this fork carry a note saying so.

## Staying in sync with upstream

`.github/workflows/upstream-sync.yml` runs every Monday (and on demand from
the Actions tab). It merges new upstream commits into the `upstream-sync`
branch, runs the test suite against PostgreSQL, and opens a pull request
into `main` stating whether the tests passed. If the merge conflicts with
this fork's own changes, it opens an issue instead. Nothing reaches `main`
until the PR is merged by hand.

The app pins a specific version of this fork and moves to a newer one only
deliberately, after review.

## Contributing back

Generic fixes (for example corrected state rate data) should also be offered
upstream as pull requests, so this fork does not have to carry them forever.
