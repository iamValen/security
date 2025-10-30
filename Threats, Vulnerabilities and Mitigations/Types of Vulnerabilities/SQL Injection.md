## Code Injection
#### Code Injection
- Adding your own information into a data stream
#### Enabled because of bad programming
- The application should properly handle input and output
#### So many different data types
- HTML, SQL, XML, LDAP, etc.


## SQL Injection
#### SQL - Structured Query Language 
- The most common relational database management system language
#### SQL Injection (SQLi)
- Put your own SQL requests into an existing application
- Your application shouldn't allow this
#### Can often be executed in a web browser
- Inject in a form or field


## Building a SQL injection
#### An example of website code
```python
"SELECT * FROM users WHERE name = '"+ username +"'"; 
```
#### How this looks to the SQL database
```SQL
SELECT * FROM users WHERE name = 'Professor'; 
```
#### Add more information to the query
```SQL
SELECT * FROM users WHERE name = 'Professor' OR '1' = '1'; 
-- ' OR '1' = '1        is the injected code
```
#### This could be very bad
- View all database information, delete database information, add user, denial of service, etc.