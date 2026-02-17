# 2. Choose Databases

Date: 2025-03-24

## Status

Accepted

## Context

As stated in a previous ADR this system will work in two components, the first one is an Administrative component where all the configuration data will be. And the second component where the "field" software will run, this field software run the attendance's part. Each component needs 
a database to connect. The first database needs to be a more robust one. It can be a RDBMS. The other database can be an embedded one.

## Decision

For the RDBMS one we choose PostgreSQL and for the embedded one we choose SQLite. This decision is made because these databases are the one that I am more familiar ones.   

## Consequences

This decision make me to implements two connections in a same project, I didn't do this before.
