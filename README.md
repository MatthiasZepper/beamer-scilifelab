## SciLifeLab Beamer Theme

A Latex Beamer theme derived from [Metropolis](https://github.com/matze/mtheme) by
Matthias Vogelsang and others and released under a [Creative Commons Attribution-ShareAlike
4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

It uses the Linux Biolinum Font Family designed by Philipp H. Poll for better readability.
The official sans-serif font specified by [SciLifeLabs visual guide](https://www.scilifelab.se/community-pages/resources/visual-identity/) is Lato designed by Łukasz Dziedzic. To use open `source/beamerfontthemescilifelab.dtx` and replace `\usepackage{biolinum}` with `\usepackage{lato}` in line 50.

## Installation

Since this theme is not on CTAN, it needs to be installed from source:

1. **Download the source** with a `git clone` of the [scilifelab repository](https://github.com/MatthiasZepper/beamer-scilifelab)
   or as a [zip archive](https://github.com/MatthiasZepper/beamer-scilifelab/archive/main.zip) of
   the latest development version.
2. **Compile the style files** by running `make sty` inside the downloaded
    directory. (Or run LaTeX directly on `source/scilifelabtheme.ins`.)
3. **Move the resulting `*.sty` files** to the folder containing your
   presentation. To use the theme with many presentations, run `make install`
   or move the `*.sty` files to a folder in your TeX path instead (might require
   `sudo` rights).
4. **Use the theme for your presentation** by declaring `\usetheme{scilifelab}` in
    the preamble of your Beamer document.
5. **For best results** install Mozilla's [Fira Sans](https://github.com/bBoxType/FiraSans).


## Usage

The following code shows a minimal example of a Beamer presentation using the theme.

```latex
\documentclass{beamer}
\usetheme{scilifelab}           % Use scilifelab theme
\title{A minimal example}
\date{\today}
\author{A Scilifelab Member}
\institute{Science for Life Laboratory}
\begin{document}
  \maketitle
  \section{First Section}
  \begin{frame}{First Frame}
    Hello, world!
  \end{frame}
\end{document}
```

## License

Like [Metropolis](https://github.com/matze/mtheme), from which it is derived,
this theme is licensed under a [Creative Commons Attribution-ShareAlike
4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/). This
means that if you change the theme and re-distribute it, you *must* retain the
copyright notice header and license it under the same CC-BY-SA license. This
does not affect the presentation that you create with the theme.
