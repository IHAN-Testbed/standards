# Data Product standards for IHAN Testbed

This repository contains Base Data Standards for IHAN Testbed.

Specification for describing data product standards can be found in
[draft/DataProducts/README.md](draft/DataProducts/README.md).

_Please note that this repository is under active development, and all the standards are
subjects to change at any time._

## Contribution guidelines

We accept contributions to this repository via
[Pull Requests](https://github.com/IHAN-Testbed/standards/pulls). You can fork the
repository, make your suggested changes in there, and then submit a Pull Request via
GitHub.

Before you submit a PR, please check that you follow these guidelines though to avoid
unnecessary work for everyone:

1. Install [pre-commit](https://pre-commit.com/#install) and make it active in your
   local clone (`pre-commit install` in repo root). Ensure this is in place BEFORE you
   make any changes, or later run `pre-commit run --all-files`.
2. Ensure your committed code follows the style guide configured in the repository
   (handled automatically by `pre-commit`)
3. Check that your naming follows existing standards. E.g. for JSON keys in Data Product
   we use `camelCase` always, do not try to submit new standards using `snake_case`.
4. Ensure you're submitting new things, i.e. check if there is an existing Data Product
   that already fits the use-case.
5. Breaking changes should be introduced via `draft`. If you want to add anything new,
   or propose a change to an existing standard that could break backwards compatibility,
   you should submit the changes in the `draft` version. Afterwards we can figure out
   which release version they can go in.

You can run the automatic validations also via Docker locally using the
`Dockerfile.validate` -configuration:

```bash
docker build . -f Dockerfile.validate
```
