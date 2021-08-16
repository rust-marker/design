[back](../README.md)

# Won't haves

Follows is a list of items that **will not** be present in the linter at any point.

- Lint implementations will not have access to the compiler's or linter's internals.
- Lint implementations will not have access to any system API provided by the linter. Access to system APIs via other methods _may_ be available, but such access is not guaranteed. Future sandboxing could result in said code erroring.
