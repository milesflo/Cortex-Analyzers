### AUTOGEN ###
# THIS FILE IS UPDATED BY `utils/dockerfile_builder.py`
# DO NOT EDIT IT DIRECTLY

# Guessing base image from source code shebang
FROM python:3-alpine

LABEL author="Emmanuel Torquato" \
      description="Check URL, file, SHA256 against ProofPoint forensics" \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="ProofPoint" \
      url="https://github.com/CERT-BDF/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . ProofPoint

# Project determined to be Python, installing deps
RUN pip install --no-cache-dir -r ProofPoint/requirements.txt

ENTRYPOINT ProofPoint/proofpoint_lookup.py