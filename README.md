# quarto_template_simple
A more simple template for making notebook style solutions of exercises with Quarto. Focus on integration with Python. This repository was made using Quarto 1.7.32. 

## Instructions for use

Shortened version of [this README](https://github.com/olivierbonte/Land_Atmosphere_interactions_notes/blob/5eb545af06890d440c73043b1e6f4ab3771a0dbe/README.md). 

First, make a local copy of this repository using

```
git clone https://github.com/olivierbonte/quarto_template_simple.git
```

or download as zip file and unzip. In each case, make sure to navigate inside the `quarto_template_simple` folder before executing any of the command line interface (CLI) instructions below.

Next, make sure you have (Mini)Conda installed (download links found [here](https://docs.anaconda.com/miniconda/)). Next open your CLI (or Anaconda prompt) and type:

```
conda env create -f environment.yml
conda activate la_interactions_quarto
```

In this repository, the final output is rendered to pdf. Therefore, [a LaTeX distribution is needed](https://quarto.org/docs/output-formats/pdf-basics.html#prerequisites). If you don't have a [Tex distribution](https://www.latex-project.org/get/#tex-distributions) installed on your machine, install the [TinyTex distribution](https://yihui.org/tinytex/), a lightweight version of [TeX Live](https://www.tug.org/texlive/), with following command in the CLI:

```
quarto install tinytex
```

There are several ways to use Quarto, but here [VS Code](https://code.visualstudio.com/Download) is used as interface. With VS Code installed for your OS, perform the following:

1. Under extensions, install the [Quarto extension](https://marketplace.visualstudio.com/items?itemName=quarto.quarto).
2. Follow the instructions [here](https://code.visualstudio.com/docs/python/environments#_select-and-activate-an-environment) and select `quarto_template_simple` as your Python interpreter for VS Code.
3. To have a nice preview of your `.qmd` quarto document, use `Ctrl + Shift + k`. After modifying the `.qmd` document, use the same key combination to render the preview again. Alternatively, run `quarto preview test_file.qmd--no-browser` in the CLI (this should normally eliminate the need to use `Ctrl + Shift + k` repeatedly).
4. To render the entire set of documents as one `.pdf`, type `quarto render test_file.qmd` in the command line. The document should be rendered to both a PDF and HTML file. 

For more details on how to use Quarto with VS Code, see the [Quarto documentation](https://quarto.org/docs/get-started/hello/vscode.html).

