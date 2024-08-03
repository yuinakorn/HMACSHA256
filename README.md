# HMACSHA256 for MySQL

Create for function name HMACSHA256 in MySQL

## Configuration

in file HMACSHA256.sql, change `root` to your own user if you want to use another user

```sql
CREATE DEFINER=`root`@`%` -- <-- here in line 1 of the file HMACSHA256.sql
```

## Execution

execute the file HMACSHA256.sql in your MySQL database


## Usage

change `your_secret` and `message_to_hash` to your own value


```sql
SELECT UPPER(HMACSHA256('your_secret', 'message_to_hash')) pass_hash
```
