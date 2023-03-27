# SQL Design
Given the following tables:

```sql
CREATE TABLE book
    {
    isbn            character varying(64) NOT NULL,
    name            character varying(64) NOT NULL,
    author_id       integer NOT NULL,
    pages           integer,
    edition         integer,
    publisher_id    integer,
    copies_sold     integer
    }
```

```sql
CREATE TABLE author
    {
    author_id       integer NOT NULL,
    name            character varying(64) NOT NULL,
    address         character varying(64),
    email           character varying(64),
    phone           character varying(64)
    }
```

```sql
CREATE TABLE publisher
    {
    publisher_id    integer NOT NULL,
    name            character varying(64) NOT NULL,
    address         character varying(64),
    email           character varying(64),
    phone           character varying(64)
    }
```

Write a SQL query statement for the following queries (don't worry about the exact syntax):

- Show me the number of books that have over 300 pages
- Give me a list of books written by Mark Boyd
- Give me a list of books written by Mark Boyd and published by Family Search
- Give me a list of books with a second edition and written by Mark Boyd and published by Family Search

Extra Credit: 
- We have millions of books in this database. What index(es) would you suggest be added.

