FROM debian:stable-slim

RUN apt-get update && apt-get install -y --no-install-recommends \
    make \
    python3 \
    python3-pip \
    texlive-latex-base \
    texlive-latex-extra \
    latexmk \
 && rm -rf /var/lib/apt/lists/*

WORKDIR /paper
