---
title: SQL injection attack
date: 2016-07-28T01:04:24.167Z
updated: 2016-07-28T01:04:00.000Z
category:
  - Security & Hacking
comments: true
---
SQL injection has become a common issue with database-driven websites. It occurs when a malefactor executes a SQL query to the database via the input data from the client to server. SQL commands are inserted into data-plane input (for example, instead of the login or password) in order to run predefined SQL commands. A successful SQL injection exploit can read sensitive data from the database, modify (insert, update or delete) database data, execute administration operations (such as shutdown) on the database, recover the content of a given file, and, in some cases, issue commands to the operating system.

For example, a web form on a website might request a user’s account name and then send it to the database in order to pull up the associated account information using dynamic SQL like this:

“SELECT * FROM users WHERE account = ‘“ + userProvidedAccountNumber +”’;”

While this works for users who are properly entering their account number, it leaves a hole for attackers. For example, if someone decided to provide an account number of “‘ or ‘1’ = ‘1’”, that would result in a query string of:

“SELECT * FROM users WHERE account = ‘’ or ‘1’ = ‘1’;”

Because ‘1’ = ‘1’ always evaluates to TRUE, the database will return the data for all users instead of just a single user.

The vulnerability to this type of cyber security attack depends on the fact that SQL makes no real distinction between the control and data planes. Therefore, SQL injections work mostly if a website uses dynamic SQL. Additionally, SQL injection is very common with PHP and ASP applications due to the prevalence of older functional interfaces. J2EE and ASP.NET applications are less likely to have easily exploited SQL injections because of the nature of the programmatic interfaces available.

In order to protect yourself from a SQL injection attacks, apply least0privilege model of permissions in your databases. Stick to stored procedures (make sure that these procedures don’t include any dynamic SQL) and prepared statements (parameterized queries). The code that is executed against the database must be strong enough to prevent injection attacks. In addition, validate input data against a white list at the application level.

Resource: blog.netwrix.com
