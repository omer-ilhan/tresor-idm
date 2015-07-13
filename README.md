# tresor-idm
Basically, keycloak preconfigured through a dockerfile. Build and run with [docker](https://www.docker.com/).

Admin Url: http://localhost:8080
Admin username & password: admin

Try out the keycloak saml authentication broker flow:

1. Visit http://localhost:8080/auth/realms/tresor-proxy-realm/protocol/openid-connect/auth?client_id=tresor-proxy&redirect_uri=http://localhost:8080/tresor-proxy/&response_type=code
2. Choose tresor-idp.
3. Log in as with username user and password user.
4. Get redirected back to given redirect_uri, in this case /tresor-proxy/.
