[[Cookie]]-based [[Authentication]] does not have solid protection against attacks, & they are mainly vulnerable to [[Cross-site Request Forgery (CSRF)]] attacks

[[Cross-site Request Forgery (CSRF)]] is where a malicious user induces another user to perform an action (clicking some virus link).

For [[Cross-site Request Forgery (CSRF)]] to occur, 3 conditions must hold:
1. Relevant action - malicious user needs to have some intention of 
2. Cookie-based session handling
3. No unpredictable request parameters