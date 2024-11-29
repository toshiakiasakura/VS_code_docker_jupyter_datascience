FROM quay.io/jupyter/datascience-notebook:x86_64-julia-1.11.1
# Note: If you change julia version, the julia version in Manifest.toml
# should be matched for building Docker image.

EXPOSE 8888
WORKDIR /workdir
COPY Project.toml Manifest.toml ./
RUN julia --project=. -e 'using Pkg; Pkg.instantiate()'

# RUN JULIA_PROJECT=/workdir
# ENV DEVCONTAINER=TRUE