### AUTOGEN ###
# THIS FILE IS UPDATED BY `utils/dockerfile_builder.py`
# DO NOT EDIT IT DIRECTLY

# Guessing base image from source code shebang
FROM python:3-alpine

LABEL author="Andrea Garavaglia, LDO-CERT" \
      description="Use Web of Trust to check a domain's reputation." \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="WOT" \
      url="https://github.com/garanews/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . WOT

# Project determined to be Python, installing deps
RUN pip install --no-cache-dir -r WOT/requirements.txt

ENTRYPOINT WOT/WOT_lookup.py