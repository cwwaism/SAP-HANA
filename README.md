# SAP-HANA
SAP HANA notes

## Get List of Users

Only list users starting with G, X or S followed by a numeric character

```
SELECT user_name FROM users 
WHERE (user_name LIKE_REGEXPR '^S\d+'
OR user_name LIKE_REGEXPR '^G\d+' 
OR user_name LIKE_REGEXPR '^X\d+')
```

