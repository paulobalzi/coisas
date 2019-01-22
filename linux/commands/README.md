### recuperar certificado de um site
```
openssl s_client -showcerts -connect meu.site.com:443 </dev/null | sed -n '/BEGIN CERTIFICATE/,/END CERTIFICATE/p' > outputfile
```
