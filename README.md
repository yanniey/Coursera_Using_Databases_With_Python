Using Database with Python

University of Michigan, 12/2016

Summary:
This is the 4th course in the Coursera specialisation: 


---


### Week 3 Multi-Table Relational SQL

Create a new table: ID(Primary Key), title(Logical Key), (album_id, genre_id as Foreign key)

```
CREATE TABLE Track (
id INTEGER NOT NULL PRIMARY KEY
AUTOINCREMENT UNIQUE,
title TEXT,
album_id INTEGER,
genre_id INTEGER,
len INTEGER, rating INTEGER, count INTEGER
)
```


```
Insert into Artist (name) values ("AC/DC");
INSERT INTO Artist (name) values ("Britney Spears")
```

Add a foreign key (a key that refers to another table)

"1" is the ID of the singer in the Artist table:

```
INSERT INTO Album (title, artist_id) values ("IV", 1)
```

JOIN, ON (~ to WHEN)

```
SELECT Album.title, Artist.name FROM Album JOIN Artist ON Album.artist_id = Artist.id

SELECT Track.title, Genre.name FROM Track JOIN Genre ON Track.genre_id = Genre.id
```

If we use JOIN without specifying an ON clause, the result will be a complete list of all possible combinations. (i.e. The number of rows you get is the number of rows in the first table times the number of rows in the second table)


Assignment: XML + SQL Database
XML: xml.etree.ElementTree Library
SQL: sqlite3 Library
---


### Week 2 Single Table Relational table with Sqlite

```
CREATE TABLE Users (
	name VARCHAR(128),
	email VARCHAR(128)
)
```

#### Insert

```
INSERT INTO Users (name,email) VALUES ("Kristine","kf@gmail.com")
```

```
INSERT INTO `courseraCourse`.`Users` (`name`, `email`) VALUES ('Anyi', 'hello@gmail.com');
```

#### Delete

```
DELETE FROM Users WHERE email="ted@gmail.com"
```

#### Update

```
UPDATE Users SET name="Charles" WHERE email="csev@gmail.com"
```

#### Select

```
SELECT * From Users
SELECT * From Users WHERE email="csev@gmail.com"
```

#### Order by

```
SELECT * From Users ORDER BY email
```

Assignment: Our First Database

```
Answer: 436F6E6C696E3135
```