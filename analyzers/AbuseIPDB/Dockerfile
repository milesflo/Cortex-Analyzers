### AUTOGEN ###
# THIS FILE IS UPDATED BY `utils/dockerfile_builder.py`
# DO NOT EDIT IT DIRECTLY

# Guessing base image from source code shebang
FROM python:3-alpine

LABEL author="Matteo Lodi" \
      description="Determine whether an IP was reported or not as malicious by AbuseIPDB" \
      license="AGPL-v3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="AbuseIPDB" \
      url="https://github.com/TheHive-Project/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . AbuseIPDB

# Project determined to be Python, installing deps
RUN pip install --no-cache-dir -r AbuseIPDB/requirements.txt

ENTRYPOINT AbuseIPDB/abuseipdb.py