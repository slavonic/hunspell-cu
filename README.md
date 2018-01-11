# hunspell-cu
Church Slavonic spelling dictionaries for Hunspell

This package provides spelling dictionaries for Church Slavonic
for [Hunspell](https://hunspell.github.io/).

## Copyright

Copyright 2018 Aleksandr Andreev.
Slavonic Computing Initiative.
Licensed under the MIT License.

## Quick Start

Copy the `cu.aff` and `cu.dic` files into the Hunspell directory
(probably `/usr/share/hunspell/`

Extensions also exist for LibreOffice and other software, which
are based on this package.

## Issues

At present, this is a poorman's spell checker:

- Cyrillic numerals may be treated as mispelled
- The dictionary does not provide any morphology

Morphological analysis for Church Slavonic is hard to do. Since
we presently don't have the resources to a write morphology into
the dictionary, the spell checker will only check the words present
in the dictionary. In other words, if the dictionary contains:

```
кни́га
кни́гꙋ
кни́зи
```

The spell checker will recognize these words, but it will treat
`кни́зѣ`, `кни́гами` and `кни́жный` as mispelled.

## Bugs in the Dictionary

Report in issue tracker.

