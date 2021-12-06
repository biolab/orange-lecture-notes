# {Orange/Quasar/Single Cell Orange} Case Study Book

![CI - PDFLatex build](https://github.com/borondics/Orange-Case-Study-Book/workflows/CI%20-%20PDFLatex%20build/badge.svg?branch=master)

Configurable teaching material for Orange and Orange-based workshops in latex.

Uses PDFLatex for compilation.

## Hints for working with Orange Lecture Notes

1. If image is placed incorrectly (i.e. doesn't align with text, flows out instead), use
```\caption{$\;$}  % empty caption for correct figure placement```
to force the image to align properly.

2. MARGINFIGURE

Figure is placed outside of the main text, has maximum width of 40mm. If larger, will overlap with body.

\begin{marginfigure}
    \centering
    \includegraphics[width=40mm]{distributions.png}
    \caption{$\;$}
    \label{fig:distributions}
\end{marginfigure}

3. WRAPFIGURE

Figure is placed outside of the main text. If larger than the width of sidenotes, figure will shrink the body of text, wrapping it around itself. The first parameter after {o} denotes the whitespace margin.

\begin{wrapfigure}{o}{0.6\textwidth}
    \includegraphics[scale=0.5]{distributions.png}
    \caption{$\;$}
\end{wrapfigure}
