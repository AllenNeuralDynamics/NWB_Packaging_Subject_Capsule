# hash:sha256:24daeda1538c49b7d05ffda5ff59131469ca92c836ab47384fe67a755a0f7ede
FROM registry.codeocean.allenneuraldynamics.org/codeocean/jupyterlab:3.6.1-miniconda4.12.0-python3.9-ubuntu20.04

ARG DEBIAN_FRONTEND=noninteractive

ARG GIT_ASKPASS
ARG GIT_ACCESS_TOKEN
COPY git-askpass /

RUN pip install -U --no-cache-dir \
    aind-data-access-api==0.6.1 \
    boto3==1.28.72 \
    hdmf-zarr==0.6.0 \
    pynwb==2.5.0
