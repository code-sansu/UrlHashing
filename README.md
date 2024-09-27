# UrlHashing

*
Create your Spring Starter Project 
Add Spring Web , H2database , Spring Data JPA , lombok dependencies
create entity class , repo class , controller class and service class same as I have made
build and run your project
Now you are all set to test the project using h2 database.

*
You can access the H2 database console via a browser to inspect the database during testing:

URL: http://localhost:8080/h2-console
JDBC URL: jdbc:h2:mem:testdb
Username: sa
Password: password

*
Write SQL queries to test such as :

1.
CREATE TABLE URL_ENTRY (
    id INT PRIMARY KEY,
    original_url VARCHAR(255),
    hashed_url VARCHAR(100)
);

2.
INSERT INTO URL_ENTRY (id, original_url, hashed_url) VALUES
(1, 'https://example.com', 'abcd1234'),
(2, 'https://example.org', 'efgh5678');

3.

SELECT * FROM URL_ENTRY;


