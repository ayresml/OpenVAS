# OpenVAS

##Files to try editing to get OpenVas to work with Postgresql
- sudo nano /etc/postgresql/13/main/postgresql.conf and change the port to 5432.
- sudo nano /etc/postgresql/12/main/postgresql.conf and change the port to 5433 (or any other port which is free).
- sudo systemctl restart postgresql
- these didn't work

###Do this
-Firstly after installing Kali-Linux-2020-3 update & upgrade

You will get this error when you attempt to install gvm

Error: the default postgresql version is not 13 required by libgvmd Use pg_upgradecluster to upgrade your Postgres cluster Which then errors out “already on version 12”

FIX: list your clusters

pg_lsclusters

and drop all clusters besides 13 cluster. eg:

sudo pg_dropcluster 12 main –stop
