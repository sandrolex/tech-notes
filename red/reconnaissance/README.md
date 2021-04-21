## TLS
    nmap --script ssl-enum-ciphers -p 8080 localhost
    
    openssl s_client -connect serverAddress:port

    openssl s_client -connect example.com:443 -tls1
    
* [sslyze](https://github.com/nabla-c0d3/sslyze)
    python3 -m sslyze [host]

* [sslscan](https://github.com/rbsec/sslscan)

## Nitko
    nikto -h host

[Nikto Cheat-Sheet](https://cdn.comparitech.com/wp-content/uploads/2019/07/NIkto-Cheat-Sheet.pdf)

* [ffuf](https://github.com/ffuf/ffuf)
* [gobuster](https://github.com/OJ/gobuster)
* [dirsearch](https://github.com/maurosoria/dirsearch)
* [rustbuster](https://github.com/phra/rustbuster)
* [feroxbuster](https://github.com/epi052/feroxbuster)

## Kiterunner
[KiteRunner](https://github.com/assetnote/kiterunner)


## APIs.Guru
[APIs.Guru](https://apis.guru/openapi-directory/)


# Enumerate subdomains
## Sublist3r
[Sublist3r](https://github.com/aboul3la/Sublist3r)

    python3 sublist3r.py -d orange.com -o orange.txt
    
    #find hosts
    #!/bin/bash

    while read sub; do
        if host "$sub" > /dev/null; then
    # If host is live, print it into
    # a file called "live.txt".
        echo "$sub" >> live-orange.txt
        #echo $sub
    fi
    done < orange.txt

## Amass
[amass](https://github.com/OWASP/Amass/blob/master/doc/install.md)
