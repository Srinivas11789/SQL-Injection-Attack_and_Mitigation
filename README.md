# Work Flow --- Attack-and-Mitigation - SQL Injection
WebServer - Django / Reverse Proxy - NGINX / Firewall - MOD Security / Attack - SQL Injection

                                 Web Application Security Analysis

----> Srinivas Piskala Ganesh Babu – spg349@nyu.edu

•	Requirements:
* A Web Page
   -Inputs a Field value
   -Outputs all the entries previously entered in the same page
*	A Web-Server Backend - Django
   -Stores the Value Returned in a database
   -Returns all the entries of the database
*	A Reverse Proxy Server – NGINX
   -A proxy server which serves the Backend Web-server
*	An SQL Injection Attack:
   -Perform an SQL Injection attack at the Server
*	A WAF – Web Application Firewall – MOD Security
   -Mitigate the SQL Injection and return 403

Output Samples:
Mod Security OFF - https://youtu.be/sF_UWBjJfX4
Mod Security ON  - https://youtu.be/fFtACyMfZQc

Work Stats:

March 21 2017 - Tuesday - 2PM - Layout of the Plan
-- Drew the Requirements
-- Assessed the work required by going through uninterrupted progress through the evening
-- NGINX Proxy without MOD Security - Done
-- Django Web Server Basic Frame - Done

March 22,23,24 - Taking a Detour - Courswork Assignments, Projects and Midterm Exams

March 25 2017 - Saturday - Start after the Detour
-- After the Morning Exam, Reworked with the work done already
-- Django Web Server Crafted with the Form and Required Output

March 26 2017 - Sunday - Attack Day
-- Started with SQL Injection Attacks
-- Setup some Raw Queries for SQLite DB that are very much vulnerable to SQL Injection Attacks
-- Performs Attacks to Delete the table from the Input Field

March 27 2017 - Monday - NGINX Reverse Proxy Setup with MOD Security
-- Proxy Settings
-- Working Frame Up
-- Mod Security Rules Analysis
-- Mitigation redirect to page 403

March 28 2017 - Tuesday - Deliver the prototype
