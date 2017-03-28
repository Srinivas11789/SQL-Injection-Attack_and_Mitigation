# SQL Inject Attack Mitigation - MOD Security WAF

--> Required: 
* Add a rule to detect the SQL Injection Attack
* Return HTTP 403 

--> Added the rule to mitigate the SQL Injection causes (In the Attack), Identified and handled DELETE in the Input

FINDINGS:
* Build MOD Security with Nginx
* Reference_Manual of MOD Security was helpful
* Reload Nginx once the Config is changed
* Config should be On for deny to work
