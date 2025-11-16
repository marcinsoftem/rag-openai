FROM python:3.11-slim

WORKDIR /app

RUN apt-get update && apt-get install -y \
    git curl build-essential bash && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

EXPOSE 8501

SHELL ["/bin/bash", "-c"]

CMD ["bash"]
