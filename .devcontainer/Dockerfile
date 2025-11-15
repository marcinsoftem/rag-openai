FROM python:3.11-slim

RUN apt-get update && apt-get install -y \
    git curl build-essential bash && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

RUN useradd -ms /bin/bash miki
USER miki

WORKDIR /workspace

EXPOSE 8501

CMD ["bash"]
