
## Proxy

### Certs
The file available at http://burpsuite/cert is also downloadable via the Proxy -> options

To make it work in ubuntu:
    man update-ca-certificates

It reads the file /etc/ca-certificates.conf line by line and add the certs

My file was in /usr/local/share/ca-certificates but  for ubuntu it needs to be in /usr/share/ca-certificates

    $ cp burp.pem /usr/share/ca-certificates/
    $ chmod 644 /usr/share/ca-certificates/burp.pem
    $ sudo update-ca-certificates
    
    $ curl https://google.com
    
Should be intercepted

File .pem and .crt are the same, just rename them

Files .req and csr also

But .der is binary

### from DER to PEM
    openssl x509 -inform der -in certificate.cer -out certificate.pem

https://www.sslshopper.com/article-most-common-openssl-commands.html



#### generate CA
    openssl req -newkey rsa:4096 -keyform PEM -keyout ca.key -x509 -days 3650 -outform PEM -out ca.cer

####generate client priv key
    openssl genrsa -out client.key 4096

#### generate cert request
    openssl req -new -key client.key -out client.req

#### sign client cert
    openssl x509 -req -in client.req -CA ca.cer -CAkey ca.key -set_serial 101 -extensions client -days 365 -outform PEM -out client.cer

#### pack into p12
    openssl pkcs12 -export -inkey client.key -in client.cer -out client.p12

#### Open SSL Cheat
https://www.makethenmakeinstall.com/2014/05/ssl-client-authentication-step-by-step/
