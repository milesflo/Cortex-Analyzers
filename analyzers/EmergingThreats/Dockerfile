FROM python:3-alpine

LABEL author="Davide Arcuri and Andrea Garavaglia, LDO-CERT" \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="EmergingThreats" \
      url="https://github.com/dadokkio/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . EmergingThreats
RUN pip install --no-cache-dir -r EmergingThreats/requirements.txt

ENTRYPOINT EmergingThreats/emergingthreats_analyzer.py