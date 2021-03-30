CSRF

3 requirements
- A relevant action 
- Cookie based session /!\ Certificate / basic auth 
- No unpredictable request parameters

SameCookies
Set-Cookie: ksjdflsd; SameSite=Strict;
Set-Cookie: ksjdflsd; SameSite=Lax;
Lax —> send the cookie only if:
GET, Top Level (click and not script)

SamSite Cookies is a protection to CSRF!


Bypass tokens:
Token depends on the method (use GET instead of POST)

Validation of token depends on the token being present !

Token is tied to the user session (like having a global table of valid tokens)

Bypass referer
Use a meta tag to ensure referer is not. sent
<meta name=“referer” content=“never”>




Cross-site scripting (or XSS) allows an attacker to execute arbitrary JavaScript within the browser of a victim user.
Cross-site request forgery (or CSRF) allows an attacker to induce a victim user to perform actions that they do not intend to.

 CSRF is one way —> the attacker can’t see the response from the request
XSS is two ways —> the attacker can read the responses from the injected script

