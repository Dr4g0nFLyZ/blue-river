```
[ req ]
distinguished_name = req_distinguished_name
x509_extensions    = v3_ca
prompt             = no

[ req_distinguished_name ]
C  = US
ST = Texas
L  = Dallas
O  = CENT
CN = Central Internal Authority

[ v3_ca ]
basicConstraints       = critical, CA:TRUE
keyUsage               = critical, digitalSignature, cRLSign, keyCertSign
subjectKeyIdentifier   = hash
authorityKeyIdentifier = keyid:always,issuer
```