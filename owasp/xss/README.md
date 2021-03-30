XSS
Is a technique for injecting javascript scripts and induce the victim to execute it
In other words, I force you to execute some malicious script
Always Client Side (browser)

Reflected
The payload is sent via the http request
http://url.com/?q=<script>alert</script>


Stored
Payload is in persistence
Second order 


DOM
Everything happens in the client side
Use the fragment 

- eval()  - innerHTML()

<script>
print(eval(value))
</script>
url/value=USER

SINK —> dangerous function
document.write()
Window.location

SOURCE —> Attacker controllable value
Document.UTL
document.baseURI location
document.cookie
window.name

Protect
—> validate input
—> encode output
—> X-Frame-Options
—> CSP
—> interHTML() / eval()


