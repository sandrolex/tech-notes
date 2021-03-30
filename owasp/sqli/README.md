SQLi

SQL injection is a web security vulnerability that allows an attacker to interfere with the queries that an application makes to its database

Blind SQL —> when the results of the attack are not returned in the application response

SELECT * FROM products WHERE category = 'Gifts'--' AND released = 1

SELECT * FROM products WHERE category = 'Gifts' OR 1=1--' AND released = 1

SELECT * FROM users WHERE username = 'administrator'--' AND password = ''


Check for ‘ and —
Try boolean 1=1 1=2


Second order SQL Injection

Stored in DB, executed later

PREVENT
—> Prepated statements

