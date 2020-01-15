# InkTeX

`InkTex` is an inkscape plugin to add `LaTeX` compiled objects to your
inkscape document.

This version is in early stages of development, but fully functional. Feel free
to try it out!

The plugin is largely inspired by the great but somewhat outdated
[textext](http://pav.iki.fi/software/textext/).

*FORK:* This fork is modified to use XeLaTeX for unicode and font support.

## Requirements

You need to have installed...

  * Python2 > 2.5
  * python-lxml
  * python-gtk2
  * pdf2svg

## Installation

### Linux

    git clone http://github.com/janoliver/inktex.git
    cd inktex
    make all

### Windows

Not supported.

## Usage

Open Inkscape and choose Extensions->InkTeX from the menu. You can set a
preamble file and scale factor in the `settings` tab. The preamble should
not include `\documentclass` and `\begin{document}`.

The LaTeX code you write is only the stuff between `\begin{document}` and
`\end{document}`. Compilation errors are reported in the `log` tab.

The preamble file and scale factor are stored on a per-drawing basis, so in a
new document, these information must be set again.
