### AUTOGEN ###
# THIS FILE IS UPDATED BY `utils/dockerfile_builder.py`
# DO NOT EDIT IT DIRECTLY

# Guessing base image from source code shebang
FROM python:3-alpine

LABEL author="Marc-Andre Doll, STARC by EXAPROBE" \
      description="Query http://www.stopforumspam.com to check if an IP or email address is a known spammer." \
      license="AGPL-V3" \
      source="https://github.com/TheHive-Project/Cortex-Analyzers" \
      title="StopForumSpam" \
      url="https://github.com/TheHive-Project/Cortex-Analyzers" \
      vendor="TheHive" \
      version="1.0.0"

WORKDIR /worker

COPY . StopForumSpam

# Project determined to be Python, installing deps
RUN pip install --no-cache-dir -r StopForumSpam/requirements.txt

ENTRYPOINT StopForumSpam/stopforumspam_analyzer.py