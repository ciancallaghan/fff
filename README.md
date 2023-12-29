# fff (Fucking Fast File-Manager)

## About

A simple file manager written in `bash`.

This is a fork of dylanaraps' original version of [fff](https://github.com/dylanaraps/fff).

- Minimal (only requires `bash` and `coreutils`)
- Works on **Linux**, **BSD**, **macOS**
- Supports `LS_COLORS`
- `cd` on exit
- Display images with `chafa`
- Supports `$CDPATH`
- Works as a file picker in `(neo)vim` ([fff.vim](https://github.com/dylanaraps/fff.vim))

## Dependencies

- `bash`
- `coreutils`

## Installation

1. `git clone https://github.com/ciancallaghan/fff`
2. `cd fff`
3. `make install`

## CD on Exit

### Bash and Zsh

```sh
f() {
    fff "$@"
    cd "$(cat "${XDG_CACHE_HOME:-${HOME}/.cache}/fff/.fff_d")"
}
```

## Example OPENER and PREVIEWER

[OPENER](./examples/opener)

[PREVIEWER](./examples/previewer)
