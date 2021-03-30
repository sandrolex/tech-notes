Host-Header

Exploits vulnerable web sites that handle the Host Header in an unsafe way
—> validate
—> escape 
—> attacker manipulate server-side behaviour 
—> X-Forwarded-For

Protect
- Don’t use it :)
- Use relative paths (/test instead of server.com/test)
- Validated it (white list)
- Don’t support override (x-)

Detect check flaws in validation GET /example HTTP/1.1
Host: hacked-subdomain.vulnerable-website.com

Duplicate
Host: vulnerable-website.com
Host: bad-stuff-here

Absolute GET https://vulnerable-website.com/ HTTP/1.1
Host: bad-stuff-here

Line Wrapping
GET /example HTTP/1.1
 Host: bad-stuff-here
Host: vulnerable-website.com

Request Smugling

Poinson Web Cache —> Use a Host Header that is not parsed by the web server, but used to build absolute paths like links to js scripts
—> Make several requests to populate the cache with links your server, where the  js has an exploit
—> If the victim hits the cache it will load the exploit

Forgot password link —> force the Host to something else and send the forgot password
—> when the real user …. 


