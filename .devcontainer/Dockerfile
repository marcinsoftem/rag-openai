FROM python:3.11-slim

WORKDIR /app

RUN apt-get update && apt-get install -y \
    git curl build-essential bash && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

COPY requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY . .

RUN useradd -ms /bin/bash miki
USER miki

EXPOSE 8501

SHELL ["/bin/bash", "-c"]

CMD ["bash"]
