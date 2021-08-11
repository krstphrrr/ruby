FROM postgres:latest

RUN apt-get update && apt-get install apt-file -y && apt-file update && apt-get install vim -y && apt-get install netcat -y

COPY ./pg/db-backups/et_audit/et_audit_2021-05-13.Thursday.sql /docker-entrypoint-initdb.d/a_et_audit_2021-05-13.Thursday.sql

COPY ./pg/db-backups/et_audit_dev/et_audit_dev_2021-05-13.Thursday.sql /docker-entrypoint-initdb.d/a_et_audit_dev_2021-05-13.Thursday.sql

COPY ./pg/db-backups/et_cache/et_cache_2021-05-13.Thursday.sql  /docker-entrypoint-initdb.d/a_et_cache_2021-05-13.Thursday.sql

COPY ./pg/db-backups/et_datamanager/et_datamanager_2021-05-13.Thursday.sql  /docker-entrypoint-initdb.d/a_et_datamanager_2021-05-13.Thursday.sql 

COPY ./pg/db-backups/et_derived/et_derived_2021-05-13.Thursday.sql /docker-entrypoint-initdb.d/a_et_derived_2021-05-13.Thursday.sql

COPY ./pg/db-backups/et_extracat/et_extracat_2021-05-13.Thursday.sql  /docker-entrypoint-initdb.d/a_et_extracat_2021-05-13.Thursday.sql

# COPY ./pg/db-backups/et_metacat/et_metacat_2021-05-13.Thursday.sql  /docker-entrypoint-initdb.d/a_et_metacat_2021-05-13.Thursday.sql

COPY ./pg/db-backups/et_user/et_user_2021-05-13.Thursday.sql  /docker-entrypoint-initdb.d/a_et_user_2021-05-13.Thursday.sql

COPY ./pg/db-backups/et_user_dev/et_user_dev_2021-05-13.Thursday.sql /docker-entrypoint-initdb.d/a_et_user_dev_2021-05-13.Thursday.sql

COPY ./pg/db-backups/postgres/postgres_2021-05-13.Thursday.sql /docker-entrypoint-initdb.d/a_postgres_2021-05-13.Thursday.sql

