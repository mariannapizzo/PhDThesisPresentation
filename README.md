# Beamer Gruvbox Theme

Modern [Beamer](https://ctan.org/pkg/beamer) themes for LaTeX presentations built around the [Gruvbox](https://github.com/morhetz/gruvbox) color palette, available in both dark and light variants.

## Features

- **GruvboxDark** — warm dark background (`#282828`), bright palette accents
- **GruvboxLight** — warm cream background (`#fbf1c7`), dark palette accents
- **Roboto Slab** for titles and headings, **Fira Sans** for body text
- Customizable accent color — change a single line to restyle the whole presentation
- Minimal chrome: thin accent bar on the title slide, separator under each frame title, clean footline
- Three block styles: standard, alert, example
- Bibliography support via **biblatex** — ready-to-use `bibliography.bib` for citations with `\cite{}`; default style is `verbose`

## Requirements

- XeLaTeX or LuaLaTeX (required for `fontspec`)
- Fonts installed on the system: [Roboto Slab](https://fonts.google.com/specimen/Roboto+Slab), [Fira Sans](https://fonts.google.com/specimen/Fira+Sans)

## Usage

```latex
\documentclass[aspectratio=169]{beamer}
\usetheme{GruvboxDark}   % or GruvboxLight
```

Compile with:

```
lualatex main.tex
```

## Accent Color

The accent color drives titles, frame title text, the separator line, bullet points, and `\alert{}`. It can be changed anywhere in the preamble`:

```latex
\usetheme{GruvboxDark}
\colorlet{gbAccentColor}{gbOrange}  % switch to orange
```

```latex
\usetheme{GruvboxLight}
\colorlet{gbAccentColor}{gbAqua} % switch to aqua
```

Implemented accent colors are `gbYellow`, `gbOrange`, `gbRed`, `gbPurple`, `gbGreen`, `gbAqua` and `gbBlue`.
