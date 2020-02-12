FROM python:3-alpine

LABEL author="Nils Kuhnert" \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="Robtex" \
      url="https://github.com/TheHive-Project/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . Robtex
RUN pip install --no-cache-dir -r Robtex/requirements.txt

ENTRYPOINT Robtex/robtex.py