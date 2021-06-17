# Why do we need this image?

We need this image because of the DataLake.

The datalake uses walk2json, which is a plugin that needs to be installed on Postgres.

With that plugin installed, debezium can connect to postgres (most likely to read service-kaizen ops)
and the datalake can receive data.

This image is a copy of https://github.com/debezium/docker-images/blob/master/postgres/11/Dockerfile with one difference,
we control the Plugin version we install

THIS IMAGE HAS BEEN EXCLUDED FROM snyk.com BECAUSE WE DO NOT USE IT ON PRODUCTION. PLEASE DO NOT USE IT ON PRODUCTION.
