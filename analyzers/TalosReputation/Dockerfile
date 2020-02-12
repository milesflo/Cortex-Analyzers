FROM python:3-alpine

LABEL author="Gabriel Antonio da Silva" \
      description="Get the Talos IP reputation" \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="TalosReputation" \
      url="https://github.com/TheHive-Project/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . TalosReputation
RUN pip install --no-cache-dir -r TalosReputation/requirements.txt

ENTRYPOINT TalosReputation/TalosReputation.py