# Vim-spell-check-files

Vim spell-check (`.spl`) files generated from Open Office dictionaries for

- Persian from [lilak](https://github.com/b00f/lilak)
- Arabic from [Dictionaries](https://github.com/titoBouzout/Dictionaries/)

as follows (following `:help mkspell` using the Persian dictionary `fa` on Unix as an example):

1. Copy the `.aff` and `.dict` files into, say `~/fa-IR`,
1. Start Vim with `LANG=fa_IR.utf-8 vim`
1. Run `:mkspell! fa ~/fa-IR` to produce `~/fa-IR/fa.utf-8.spl`.
    In case of error codes, say `E783`, adapt (or simply remove) lines in the `.aff` file that produces these (as hinted by `:help E783`) and retry.

# Caveat

These dictionary files are incomplete and erroneous.
They hopefully serve as a starting point for future improvements by others better versed in Vim spell-check file creation.
Pull requests are most welcome!

# Related

A Turkish spell-check files is available at [turiksh-spl-file-vim](https://github.com/fatihkaan22/turiksh-spl-file-vim).
