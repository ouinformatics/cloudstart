Google Compute Engine
=====================

Use instructions [here](http://docs.ansible.com/guide_gce.html) to setup

Export pkcs12 auth file from GCE dashboard and create auth.pem and place in this director, then eddit vars.yml to match your account and desired configuration.
```
openssl pkcs12 -in pkey.pkcs12 -passin pass:notasecret -nodes -nocerts | openssl rsa -out auth.pem
```
