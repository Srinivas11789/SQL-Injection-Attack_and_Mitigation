# SQL Inject Attack Mitigation - MOD Security WAF

--> Required: 
* Add a rule to detect the SQL Injection Attack
* Return HTTP 403 

--> Added the rule to mitigate the SQL Injection causes (In the Attack), Identified and handled DELETE in the Input

RULES ADDED:

--> To prevent SQL Multiple Query or Stacked Query Attack

SecRule ARGS:Entry "@rx (?i:delete)|(?i:select)|(?i:insert)|(?i:drop)|(?i:union)|(?i:join)|(?i:alter)" "id:13,msg:'SQL Injection Multi Query',severity:ALERT,deny,status:403"

SecRule REQUEST_URI|ARGS|ARGS_NAMES "@detectSQLi" "id:152,deny,status:403"

SecRule ARGS:Entry "@contains delete" "id:11,msg:'SQL Injection Multi Query',severity:ALERT,deny,status:403"

Issue Fix:

SecRule ARGS:Entry "@rx (?:')" "id:12,msg:'SQL Injection Multi SPL Query',severity:ALERT,deny,status:403"

FINDINGS:
* Build MOD Security with Nginx
* Reference_Manual of MOD Security was helpful
* Reload Nginx once the Config is changed
* Config should be On for deny to work
