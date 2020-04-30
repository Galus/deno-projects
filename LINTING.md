# Deno Lint

The community is already asking for a linter, and asking for eslint support.
The TLDR is that the community wants to standardize their own linter rather
than having to support multiple linters and code styles. Already a lint project
is being developed @ https://github.com/denoland/deno_lint 
https://github.com/denoland/deno/issues/1880

# Setting up Deno Lint
The [Deno Lint](https://github.com/denoland/deno_lint) project is a rust crate that needs to be built with rust's `cargo`

When the executable linter is available on the path, then it may be configured as the linter of choice:

vim ex.: 
```
let g:ale_fixers = {
     \ '*': ['remove_trailing_lines', 'trim_whitespace'],
     \ 'javascript': ['eslint'],
     \ 'typescript': ['denolint']
```
