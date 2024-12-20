FROM quay.io/jupyter/datascience-notebook:julia-1.10.5
# Note: If you change julia version, the julia version in Manifest.toml
# should be matched for building Docker image.
# Note: julia-1.11.1 has a slow launch time, change it to julia-1.10.5
# and wait for a new release for 1.11.

EXPOSE 8888
WORKDIR /workdir
COPY Project.toml Manifest.toml ./
RUN julia --project=. -e 'using Pkg; Pkg.instantiate()'

# RUN JULIA_PROJECT=/workdir
# ENV DEVCONTAINER=TRUE