[back](./README.md)

# Could haves

Follows is a list of items that **may** be present in the minimum viable product of a custom linter. Items would be nice to have, but are not expected to be implemented; they are most likely to be long-term goals and implemented at a later date.

- Lints could be easily testable. [`compiletest-rs`](https://github.com/Manishearth/compiletest-rs) and [`trybuild`](https://github.com/dtolnay/trybuild) can serve as inspiration.
- Lints could be run in parallel. Care should be taken to ensure this does not negatively interact with the aforementioned tester, specifically the ordering of lint outputs.
