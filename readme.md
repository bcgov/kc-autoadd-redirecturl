
[![Issues](https://img.shields.io/github/issues/bcgov/kc-autoadd-redirecturl)](/../../issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/bcgov/kc-autoadd-redirecturl)](/../../pulls)
[![MIT License](https://img.shields.io/github/license/bcgov/kc-autoadd-redirecturl.svg)](/LICENSE)
[![Lifecycle:Retired](https://img.shields.io/badge/Lifecycle-Retired-d45500)](https://github.com/bcgov/repomountie/blob/master/doc/lifecycle-badges.md)

# Add Keycloak Redirect

## setup - install deps

```
python -m venv venv
. ./venv/bin/activate
pip install -r requirements.txt
```

## setup - define env vars

* define the following environment variables:
```
KC_HOST=<keycloak host>
KC_CLIENTID=<keycloak client id with service account>
KC_SECRET=<keycloak secret>
KC_REALM=<keycloak realm>

KC_CLIENT_2_CONFIG=<keycloak client who's redirect urls are to be modified>
```

## Add Redirect:

`python src/keyCloakAddRedirect.py -add redirect_url`

## Remove Redirect:
`python src/keyCloakAddRedirect.py -del redirect_url`

