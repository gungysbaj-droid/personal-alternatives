# Personal Alternatives

A growing library of original open-source apps and reusable components.

The aim is to understand useful software behaviors, build independent implementations, and keep the code portable enough to reuse across future projects.

## Layout

- `apps/`: standalone apps, each with its own README, tests, and build instructions.
- `packages/`: reusable components extracted from working apps.
- `docs/`: workflow, provenance, and maintenance rules.
- `templates/`: a brief to complete before starting an implementation.

No first app has been selected yet. This is a project scaffold, not a working alternative app.

## Workflow

1. Pick one useful behavior and define an acceptance test.
2. Check the permissions and terms for any target or reference material.
3. Inspect only authorized inputs. REA can help gather evidence where appropriate.
4. Write an independent implementation and test it against the agreed behavior.
5. Check dependencies, licenses, and private data before publication.
6. Extract a reusable component only after an app demonstrates its usefulness.

See [the implementation brief](templates/implementation-brief.md) and [provenance rules](docs/provenance.md).

## REA

[REA](https://github.com/morluto/rea) is an optional analysis tool, not the foundation of every app. Its own code is [MIT licensed](https://github.com/morluto/rea/blob/main/LICENSE). This library does not include REA code or code recovered from other applications.

REA's license does not license the software it analyzes. A public implementation must contain original code or material whose license permits the intended reuse, with required notices preserved. No license bypasses, copied proprietary code, or proprietary assets belong here.

## Long-term use

Keep a local clone and a separate backup. Each app should record its dependencies and tested tool versions, include an offline/local usage path where practical, and document how to export its data. Pin dependencies and test upgrades. Public hosting alone does not guarantee indefinite availability.

## License

Original material in this repository is licensed under MIT; see LICENSE. Third-party code and assets retain their own licenses.
