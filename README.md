# OpenVAS

##Files to try editing to get OpenVas to work with Postgresql
- sudo nano /etc/postgresql/13/main/postgresql.conf and change the port to 5432.
- sudo nano /etc/postgresql/12/main/postgresql.conf and change the port to 5433 (or any other port which is free).
- sudo systemctl restart postgresql
