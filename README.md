# Textlint Plugin LaTeX2ε
[![npm](https://img.shields.io/npm/v/@ta2gch/textlint-plugin-latex2e.svg)](https://www.npmjs.com/package/@ta2gch/textlint-plugin-latex2e)
[![circleci](https://img.shields.io/circleci/project/github/ta2gch/textlint-plugin-latex2e.svg)](https://circleci.com/gh/ta2gch/textlint-plugin-latex2e)


This plugin contains rough LaTeX parser which doesn't cover all syntax, but it's enough.

We welcome your contribution for adding new syntax! Thanks.

## Installation

```
$ npm install @ta2gch/textlint-plugin-latex2e
```

And add to `.textlintrc`

```
   plugins: ["@ta2gch/textlint-plugin-latex2e"]
```

## Known Issue

This kind of syntax cannot be interpreted correctly.

```latex
\newenvironment{A}
{\begin{B}}
{\end{B}}
```

To avoid this issue, you can write them out of the file with `\input` command.

## Roadmap

- [ ] Add tests (Currently works well for me but no tests)
    - [ ] Comment
    - [ ] Macro
    - [ ] Verbatim
    - [ ] Environment
    - [ ] DisplayMath
    - [ ] InlineMath
    - [ ] Document

- [ ] Skip some component with `.textlintrc`.
    - [ ] Macro
    - [ ] Environment

## Copyright

Copyright (C) 2018 TANIGUCHI Masaya ALL Rights Reserved.

## License

This software is licensed under the GPLv3 or later.
