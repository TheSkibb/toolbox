# connect nifi to postgres

## postgres server

start postgres server. for example using a podman container

## JDBC driver

download the postgresql JDBC driver from https://jdbc.postgresql.org/

put the jar file in <location of nifi>/lib/

## create a connection pool

right click nifi workspace -> controller services

click + button top right

select DBCP connection pool

click the three buttons on right of service -> edit

set properties of service
    - database connection url: jdb:postgresql://<location of postgres>:<port>/<database name>
    - database driver class name: org.postgresql.Driver
    - database driver location: <location of nifi>/lib/postgresql<version number>.jar
    - database user: <username>
    - Password: <password> (may be wise to use nifi secrets)

close the configuration window and press the three buttons -> enable

if anything goes wrong during the enabling process, it will show up as a little mark on the left side of the service. You can also use the bulletin board for monitoring these error messages.

## do sql queries

Add a processor like ExecuteSQL and set the "Database Connection Pooling Service" to be the service you just created.

