# Contributing to PlatformKit OSS

Thanks for helping shape the PlatformKit open-source ecosystem.

## Where to start

- **Questions and discussions:** Use [GitHub Discussions](https://github.com/septagon-dev/platformkit-community/discussions) — not issues.
- **Bug reports:** Open a GitHub issue in the affected repository.
- **Documentation improvements:** Open a PR in [`pk-docs`](https://github.com/septagon-oss/pk-docs).
- **Module or core changes:** Open a PR in the relevant repo (`pk-core`, `pk-modules`, etc.).

## Working rules

1. **Keep repository boundaries explicit.** Every repository has a `REPO_CHARTER.md` defining its scope. If your change crosses a boundary, it probably belongs in a different repo.
2. **Use conventional commits.** `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `ci:`, `chore:` — with the repo as scope (e.g. `feat(pk-core):`).
3. **Prefer small pull requests.** A PR that touches 3–10 files is easier to review than one that touches 30.
4. **Run `make verify` before pushing.** Each repo defines its own verification pipeline (tests + vet + lint). Need the go.work set up? See each repo's README.
5. **Module authors: no direct imports across modules.** If you're building a new PlatformKit module, it must communicate through declared ports/interfaces, never by importing another module's implementation.

## Pull request checklist

- Scope is clearly within the repository's boundary
- `REPO_CHARTER.md` is updated if the change shifts scope
- All CI checks pass
- Documentation is updated when behaviour or boundaries change

## Code of Conduct

By participating, you agree to the [Code of Conduct](CODE_OF_CONDUCT.md).

## License

All contributions are licensed under Apache 2.0.
