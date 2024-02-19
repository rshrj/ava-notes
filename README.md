# High Energy Theory LaTeX Template

This LaTeX template is designed for high energy theoretical physics papers, providing an aesthetically pleasing layout that adheres to the typical structure of scientific publications. It includes predefined sections, figure and table integration, reference management, and more, aiming to facilitate the writing process and ensure that your documents are both professional and visually appealing.

## Features

- **Customizable Layout**: Easily adjust margins, headers, footers, and more.
- **Integrated Bibliography Management**: Choose between `BibTeX` or `biblatex` for handling references.
- **Figure and Table Support**: Predefined commands for including and referencing figures and tables.
- **Code and Algorithm Formatting**: Tools for including code snippets and algorithms.
- **Cross-Platform Compatibility**: Works seamlessly across different LaTeX editors and compilers.

## Getting Started

### Prerequisites

Ensure you have a LaTeX distribution installed, such as [TeX Live](https://tug.org/texlive/), [MiKTeX](https://miktex.org/), or [MacTeX](http://www.tug.org/mactex/), and a preferred editor (e.g., VSCode w/ LaTeX Workshop, TeXstudio, Overleaf).

### Installation

Clone this repository or download the ZIP file to get started:

```
git clone https://github.com/rshrj/ava-notes.git
```

Navigate to the template directory:

```
cd ava-notes
```

### Using the Template

1. **Edit the `.tex` file**: Open the template `.tex` file in your LaTeX editor.
2. **Customize as needed**: Modify the document sections, add your content, figures, tables, and references as per your requirements.
3. **Compile the document**: Use your LaTeX editor or command line to compile the `.tex` file into a PDF. For example, using `latexmk`:
```bash
$ latexmk \
    --max-print-line=10000 \
    -synctex=1 \
    -interaction=nonstopmode \
    -file-line-error \
    -pdf \
    -outdir=./build \
    ./main
```

## Structure

The template includes the following sections:

- Introduction
- Methods
- Results
- Discussion
- Conclusions
- Acknowledgments
- References

## Adding Figures and Tables

To include a figure, use the following syntax:

```latex
\begin{figure}[ht]
\centering
\includegraphics[width=0.5\textwidth]{path/to/your/figure.png}
\caption{Figure caption.}
\label{fig:your-label}
\end{figure}
```

For tables, use:

```latex
\begin{table}[ht]
\centering
\begin{tabular}{|l|c|r|}
\hline
Column 1 & Column 2 & Column 3 \\
\hline
Data 1 & Data 2 & Data 3 \\
\hline
\end{tabular}
\caption{Table caption.}
\label{tab:your-label}
\end{table}
```

## Managing References

This template supports both `BibTeX` and `biblatex` for managing references. See the included sample `.bib` file for formatting examples.

## Contributing

Contributions to improve the template are welcome! Feel free to fork the repository, make changes, and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## Acknowledgments

- [TODO] Acknowledge any projects, individuals, or organizations that helped inspire or contribute to the template.