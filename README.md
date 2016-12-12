

Week 2

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