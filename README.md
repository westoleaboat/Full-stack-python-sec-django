# Full-stack-python-sec-django

pipenv graph - to show installed dependencies 

generate a key pair and a self-signed public-key certificate with the following openssl command.

### this example generates an elliptic-curve key pair and a self-signed public-key certificate, valid for 10 years

'''
openssl req -x509 -nodes -days 3650 -newkey ec:<(openssl ecparam -name prime256v1) -keyout private_key.pem -out certificate.pem
'''

X.509 certificate
validity period 10 years
generates an elliptic-curve key pair
writes the private key
writes the public key certificate

## The Strict-Transport-Security response header
A server uses the HTTP Strict-Transport-Security (HSTS) response header to
tell a browser that it should be accessed only via HTTPS. For example, a server would
use the following response header to instruct the browser that it should be accessed
only over HTTPS for the next 3600 seconds (1 hour):
Strict-Transport-Security: max-age=3600
The key-value pair to the right of the colon, shown in bold font, is known as a directive.
Directives are used to parameterize HTTP headers. In this case, the max-age directive
represents the time, in seconds, that a browser should access the site only over HTTPS.
