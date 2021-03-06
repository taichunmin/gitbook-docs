# H.4. Extensions

PostgreSQL is designed to be easily extensible. For this reason, extensions loaded into the database can function just like features that are built in. The `contrib/` directory shipped with the source code contains several extensions, which are described in [Appendix F](https://www.postgresql.org/docs/10/static/contrib.html). Other extensions are developed independently, like [PostGIS](http://postgis.net/). Even PostgreSQL replication solutions can be developed externally. For example, [Slony-I](http://www.slony.info/) is a popular master/standby replication solution that is developed independently from the core project.

