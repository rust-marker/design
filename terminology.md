[back](./README.md)

# Terminology

**Linter** or **lint tool**: The program called by the user, generally via command line or in CI. Configuration may or may not be provided as command line parameters.

**Driver**: The internal code that loads and executes various lints. _Not_ the lints themselves.

**Lint package** or **lint crate**: A set of lints provided as a single library, whatever form that ultimately takes. Likely forms a namespace (such as `foo::*` for the `foo` crate).

**Lint implementation**: A dynamically loadable lint. Part of a lint package.

**Lint group**: A set of lints within a lint package that are related in some way. The grouping is defined by the lint package author.

**End user** or **lint user**: The person who calls the linter from the command line. Output is displayed to this user.
