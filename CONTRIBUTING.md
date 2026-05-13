# Contributing to Angular CLI

We would love for you to contribute to this project and help make it even better than it is today!
As a contributor, here are the guidelines we would like you to follow:

## Code of Conduct

Please read and follow our [Code of Conduct](CODE_OF_CONDUCT.md).

## Found a Bug?

If you find a bug in the source code, you can help us by [submitting an issue](https://github.com/angular/angular-cli/issues/new?template=1-bug-report.yml).
Even better, you can submit a Pull Request with a fix.

## Missing a Feature?

You can *request* a new feature by [submitting an issue](https://github.com/angular/angular-cli/issues/new?template=2-feature-request.yml).
If you would like to *implement* a new feature, please consider the size of the change:

- For a **major feature**, first open an issue and outline your proposal so it can be discussed.
- **Small features** can be crafted and directly submitted as a Pull Request.

## Submission Guidelines

### Submitting an Issue

Before you submit an issue, please search the issue tracker. An issue for your problem might already exist and the discussion might inform you of workarounds readily available.

### Submitting a Pull Request (PR)

Before you submit your Pull Request (PR) consider the following guidelines:

1. Search [GitHub](https://github.com/angular/angular-cli/pulls) for an open or closed PR that relates to your submission.
2. Be sure that an issue describes the problem you're fixing, or documents the design for the feature you'd like to add.
3. Fork the repo.
4. Make your changes in a new git branch:

   ```shell
   git checkout -b my-fix-branch main
   ```

5. Create your patch, **including appropriate test cases**.
6. Follow our [Coding Rules](#coding-rules).
7. Run the full test suite and ensure all tests pass.
8. Commit your changes using a descriptive commit message that follows our [commit message conventions](#commit-message-format).
9. Push your branch to GitHub:

   ```shell
   git push origin my-fix-branch
   ```

10. In GitHub, send a pull request to `angular-cli:main`.

## Coding Rules

To ensure consistency throughout the source code, keep these rules in mind as you are working:

- All features or bug fixes **must be tested** by one or more specs (unit-tests).
- All public API methods **must be documented**.
- We follow [Google's JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html).

## Commit Message Format

We have very precise rules over how our Git commit messages must be formatted.
This format leads to **easier to read commit history**.

Each commit message consists of a **header**, a **body**, and a **footer**.

```
<type>(<scope>): <short summary>
  │       │             │
  │       │             └─⫸ Summary in present tense. Not capitalized. No period at the end.
  │       │
  │       └─⫸ Commit Scope: animations|bazel|benchpress|common|...
  │
  └─⫸ Commit Type: build|ci|docs|feat|fix|perf|refactor|test
```

### Type

Must be one of the following:

- **build**: Changes that affect the build system or external dependencies
- **ci**: Changes to our CI configuration files and scripts
- **docs**: Documentation only changes
- **feat**: A new feature
- **fix**: A bug fix
- **perf**: A code change that improves performance
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **test**: Adding missing tests or correcting existing tests

## Setting Up Your Development Environment

### Prerequisites

- Node.js (see `.nvmrc` for the required version)
- Yarn package manager
- Bazel (see `.bazelversion` for the required version)

### Installation

```shell
# Clone the repository
git clone https://github.com/<your-fork>/angular-cli.git
cd angular-cli

# Install dependencies
yarn install
```

### Running Tests

```shell
# Run all tests
yarn test

# Run tests with Bazel
bazel test //...
```

## License

By contributing to Angular CLI, you agree that your contributions will be licensed under the [MIT License](LICENSE).
