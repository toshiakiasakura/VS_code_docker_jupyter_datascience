# Boilerplate for VS code environment for data analysis.

This boilerplate is prepared to develop the code
in Python, R, and Julia using the Jupyter datascience notebook image,
and opens files with .ipynb extension within VS code.

Key files are `.devcontainer/Dockerfile` and `.devcontainer/devcontainer.json`.

## Package version management.
The package version management relies on each language's
package designed for that purpose, and information is cached in a local environment.

Specifically,
- Python: `requirements.txt` and `pip`,
- R: `renv`,
- Julia: `Project.toml`.

## Note
THe extensions for each package should be installed for running in the jupyter notebook.
Also, for R language, `Jupyter` extension may need to switch to the pre-release version.

## Installed extensions
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







