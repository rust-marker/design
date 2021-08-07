[back](./README.md)

# Must haves

Follows is a list of items that **must** be present in the minimum viable product of a custom linter.

- The linter must be able to run in CI. This does not necessarily mean that it is trivial to do so. A demonstration should likely be provided.
- Lints implementations must have access to type information.
- The end user must be able to change the severity of lints that are not `#[forbid(...)]` by default.
- The lint author must be able to write lints without knowing the implementation details of anything, including the stable API, rustc crates, or the standard library.
- The lint user must be able to use the lints without knowing the implementation details of the linter.
- All lint implementations must be able to work with a single driver which is provided by the linter.
- Lints must be able to be forbid, deny, warn, and allow-by-default.
