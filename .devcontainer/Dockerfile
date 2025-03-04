FROM python:3.13.2-slim

RUN adduser -q --gecos "" --disabled-password mkuser \
    && apt-get update \
    && apt-get install -y --no-install-recommends git build-essential \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

USER mkuser

RUN pip install --upgrade pip \
    && pip install --no-cache-dir mkdocs mkdocs-material fontawesome-markdown mdx_unimoji python-markdown-math pymdown-extensions \
    mkdocs-pdf-export-plugin \
    mkdocs-git-revision-date-localized-plugin \
    mkdocs-minify-plugin \
    markdown-include

USER root
