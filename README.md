# coq.nvim Thirdparty Sources

Shim layer for [`coq.nvim`](https://github.com/ms-jpq/coq_nvim) to communicate with other vim plugins.

See [`:COQhelp custom_sources`](https://github.com/ms-jpq/coq_nvim/tree/coq/docs/CUSTOM_SOURCES.md)

## How to use

Install the repo the normal way, and then:

```lua
require("coq_3rd") {
  { src = "demo" },
  { src = "vimtex", short_name = "vTEX" },
  ...
}
```

`require("coq_3rd")` takes a list of `{ src = ..., short_name = ..., ... }` objects.

`src` is required

If `short_name` is not specified, it is uppercase `src`.

The rest of object are specific to each individual source.

## Sources

### Demo

`{ src = "demo" }`

This is a reference implementation, do not enable it unless you want to write your own plugin, and want to see how it works.

### [VimTex](https://github.com/lervag/vimtex)

`{ src = "vimtex" }`
