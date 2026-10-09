# Contributing to Project Colony

This guide applies to every repository in the Project-Colony organization that
does not ship its own `CONTRIBUTING.md`. How to build and test a project is in
that repository's README or `docs/`.

## Before you start

- A bug fix or a small change can go straight to a pull request.
- For a new feature or a large change, open an issue first, so the approach is
  agreed on before you write the code.
- Never report a security problem in a public issue or pull request. Report it
  privately, as described in [SECURITY.md](SECURITY.md).

## Pull requests

- **One coherent change per pull request.** Unrelated fixes go in separate pull
  requests.
- **The pull request title is the changelog entry.** Pull requests are
  squash-merged under their title, and release-please derives the next version
  and the changelog from it. Write the title as a
  [conventional commit](https://www.conventionalcommits.org/) that a user can
  understand:

  ```text
  feat: import playlists from M3U files
  fix(settings): keep the chosen theme after a restart
  ```

  The usual types are `feat`, `fix`, `perf`, `refactor`, `docs`, `test`,
  `build`, `ci` and `chore`. A breaking change adds `!` after the type, as
  in `feat!: drop the old settings format`.
- **Commit messages** follow the same convention.
- **Tests:** run the repository's checks before you open the pull request, and
  add tests for new logic.
- **Documentation:** a change that makes a README or `docs/` page wrong updates
  that page in the same pull request.

## Language

Everything in a repository is written in English: code, comments, commit
messages, pull requests, issues and documentation. French appears only as a
translation of a program's interface.

## Authorship

Commits and pull requests carry no AI credits: no `Co-Authored-By` trailer for
an AI tool, no "generated with" footer. Do not commit agent files either, such
as `CLAUDE.md`, `AGENTS.md`, `.claude/`, `.cursor/`, or prompts, plans and
reports written by an agent.

## License

By contributing, you agree that your contribution is licensed under the license
of the repository it goes into: GPL-3.0-or-later, except for SAM - Colony
Edition, which is GPL-3.0-only.
