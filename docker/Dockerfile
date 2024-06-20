FROM ubuntu:22.04
RUN apt-get update && apt-get install -y nano jq curl wget python3-pip && pip install llm-shell weasel stonemill
RUN curl -sL https://deb.nodesource.com/setup_20.x | bash
RUN apt update && apt install -y git nodejs && npm install --global rollup
WORKDIR /app
CMD ["bash"]
