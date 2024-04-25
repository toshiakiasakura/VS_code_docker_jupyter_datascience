# Boilerplate for the VS code environment for data analysis.

This boilerplate was prepared to develop the code
in Python, R, and Julia using the Jupyter datascience notebook docker image,
and enabling working on files with .ipynb extension within VS code.

Two key files are `.devcontainer/Dockerfile` and `.devcontainer/devcontainer.json`.

## Package version management.
The package version management relies on each language's
package designed for that purpose, and
that package information is cached in a local environment.

Specifically,
- Python: `requirements.txt` and `pip`,
- R: `renv`,
- Julia: `Project.toml`.

## Note
The extensions for each package should be installed to run the code in the jupyter notebook.
Also, for the R language, you may need to switch
the version of the `Jupyter` extension to the pre-release one.

## Installed extensions.
Jupyter
- Jupyter (may need the pre-release version): "ms-toolsai.jupyter",
- Jupytext: "donjayamanne.vscode-jupytext",

Julia
- Julia extension: "julialang.language-julia"
- Julia formater: "0h7z.vscode-julia-format"

R
- R: "REditorSupport.r",
- R debugger: "RDebugger.r-debugger",

Python
- "ms-python.python",

General
- Grammarly for VS code: "znck.grammarly",
- Edit csv: "janisdd.vscode-edit-csv",