FROM python:3-alpine

LABEL author="Nils Kuhnert, CERT-Bund" \
      description="Check if ip is sinkholed via sinkdb.abuse.ch" \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="SinkDB" \
      url="https://github.com/BSI-CERT-Bund/sinkdb-analyzer" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . SinkDB
RUN pip install --no-cache-dir -r SinkDB/requirements.txt

ENTRYPOINT SinkDB/sinkdb.py