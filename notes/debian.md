# Debian Server

Na debian serveru jsem rozchodil klasický Apache2 webserver. \
Zlepšil jsem kvalitu ssh, provedl základní nastavení bezpečného ssh:
- zakázal jsem root login
- autorizace pouze pomocí ssh klíčů


## Co na serveru?

Debian server využiju jako host pro konteinerizované zranitelné webové aplikace. Jako je například DVWA nebo WebGoat

### DVWA [(github)](https://github.com/digininja/DVWA)
DVWA (tedy damn vulnerable web application) je webová aplikace, která je záměrně zranitelná a ulehčuje pochopení základních bezpečnostních rizik OWASP.
(Brute force, Command Injection, SQL Injection, JavaScript, File Upload a podobné) \
Má skvělou funkci nastavení úrovně zabezpečení, která nabízí rychlé přenastavení zabezpečení serveru a tedy náročnost na využití daného zranitelného místa.

## Co je v plánu?
Původní nápad celého takového serveru je zkusit nějaké zranitelná místa využít a zkontrolovat logy. V tomto plánu mi pomůže operační systém **Kali Linux**, který nabízí předinstalované penetrační nástroje. Pochopit co se v realitě na serveru děje. Tyto dané děje budu dokumentovat a zaznamenávat zde na vedlejší stránce.
