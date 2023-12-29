# HMACSHA256 for MySQL

Create for function name HMACSHA256 in MySQL

## Configuration

in function HMACSHA256, change `your_user_here` to your own user

```sql
CREATE DEFINER=`your_user_here`@`%` FUNCTION `HMACSHA256`(secret_key VARCHAR(256), val VARCHAR(2048)) RETURNS char(64) CHARSET utf8
```

## Usage

change `your_secret` and `message_to_hash` to your own value


```sql
SELECT UPPER(HMACSHA256('your_secret', 'message_to_hash')) pass_hash
```
