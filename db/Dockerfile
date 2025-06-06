FROM postgres:13-alpine3.22

ENV POSTGRES_HOST_AUTH_METHOD=trust

COPY ./words.sql /docker-entrypoint-initdb.d

EXPOSE 5432
