# SQL Injection Attack

* A Html Page with a Field Provision has been given wherein any input can be validated. 
Hint: Had used a Raw SQL Query in the Server

* Identify a Input which may allow to perform actions other than anticipated

-----> Input Selected: < 4';delete from 'entries_entry >
This input add the content 4 and deletes all the table entries.

Findings:
- Django DB Driver properly handles and escapes the SQL Query, Hence used a Raw Query for the given prototype


