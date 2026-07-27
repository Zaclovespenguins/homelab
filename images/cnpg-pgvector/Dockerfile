ARG PG_MAJOR=17
FROM ghcr.io/cloudnative-pg/postgresql:${PG_MAJOR}-bookworm
USER root
RUN apt-get update \
 && apt-get install -y --no-install-recommends postgresql-${PG_MAJOR}-pgvector \
 && rm -rf /var/lib/apt/lists/*
USER 26
