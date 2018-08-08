# MariaDB

The following are the documentation to work with the database.

## Data Schema

### Person

| Field       | Type         | Null | Key | Default | Extra |
| ----------- | ------------ | ---- | --- | ------- | ----- |
| id          | int(11)      | NO   | PRI | NULL    |       |
| name        | varchar(100) | NO   |     | NULL    |       |
| email       | varchar(100) | NO   |     | NULL    |       |
| phonenumber | varchar(100) | NO   |     | NULL    |       |

## Usage

### Initialize database

```sql
CREATE contacts; --Create database named contacts
USE contacts;
```

### Create table

```sql
CREATE TABLE person (
   id INT NOT NULL AUTO_INCREMENT,
   name VARCHAR(100) NOT NULL,
   email VARCHAR(100) NOT NULL,
   phonenumber VARCHAR(100) NOT NULL,
   PRIMARY KEY(id)
);
```

### Delete table

```sql
DELETE TABLE person;
```

### Insert data into the table

```sql
INSERT INTO person (id, name, email, phonenumber) VALUES ('2', 'Odin', 'odin@asgard.com', '+00 231 1242 21');
```

### Show all data from the table

```sql
SELECT * FROM person;
```

### Delete data from the table based on data's id

```sql
 DELETE FROM person WHERE id=2; --delete data with 2 as the id number
```

### Delete all data from the table

```sql
DELETE * FROM person;
```
