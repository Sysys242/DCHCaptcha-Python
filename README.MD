# Py-DCHcaptcha

A simple python wrapper for [dchcaptcha.com](https://dchcaptcha.com/).

## Setup
### PIP doesn't work anymore ( azulax wanted me to delte it ): please download sources.
### Modules required: tls_client

## How to use
```python
from py_dchcaptcha import DCHcaptcha

dch = DCHcaptcha('api_key')

key = dch.solve(
    'site_key', # HCaptcha site key of your website.
    'link', # Link of the page where you are solving it.
    'proxy', # HTTP Proxy, format: user:pass@ip:port or ip:port
    'rqdata' # Optional, used for silent captcha, ex: discord join.
)
print(key)
```
