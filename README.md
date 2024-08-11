# apisix

API Gateway for the NRDB API, using APISIX.

## Environment 

This setup needs an environment file in `.env` to configure it.

### Required Fields

```
APISIX_STAND_ALONE=true
KEYCLOAK_URL=https://keycloak-domain/realms/your-realm/.well-known/openid-configuration
KEYCLOAK_CLIENT_ID=client-id-for-keycloak-oauth-client
KEYCLOAK_SECRET=client-secret-for-keycloak-oauth-client
```

### Optional Fields

If using the nginx-proxy configuration, also add config for it:

```
VIRTUAL_HOST=the-domain.com
VIRTUAL_PORT=9080
LETSENCRYPT_HOST=the-domain.com
LETSENCRYPT_EMAIL=email@the-domain.com
```
