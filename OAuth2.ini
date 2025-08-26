OAuth2 Flow Test Documentation

Password Grant Flow
POST /token
Request Body (x-www-form-urlencoded):
grant_type=password
client_id=web-app
client_secret=srqqsYGgUlMdUOgAqt1utrHEOhZTXCES
username=user3
password=12345
scope=openid

Response:
{
  "access_token": "<JWT_ACCESS_TOKEN>",
  "expires_in": 300,
  "refresh_token": "<JWT_REFRESH_TOKEN>",
  "token_type": "Bearer",
  "id_token": "<JWT_ID_TOKEN>",
  "scope": "openid email profile"
}

Client Credentials Flow
POST /token
Request Body (x-www-form-urlencoded):
grant_type=client_credentials
client_id=web-app
client_secret=srqqsYGgUlMdUOgAqt1utrHEOhZTXCES

Response:
{
  "access_token": "<JWT_ACCESS_TOKEN>",
  "expires_in": 300,
  "token_type": "Bearer"
}

Authorization Code Flow
GET /auth
Request URL:
http://localhost:8080/realms/Dmytro/protocol/openid-connect/auth?response_type=code&client_id=web-app&redirect_uri=https://oauth.pstmn.io/v1/callback&scope=openid

Після цього користувача буде перенаправлено на сторінку входу. 
Після успішного входу, користувача буде перенаправлено на redirect_uri. 
Далі потрібно обміняти отриманий код на токен за допомогою POST /token.

Response:
{
  "access_token": "<JWT_ACCESS_TOKEN>",
  "expires_in": 300,
  "refresh_token": "<JWT_REFRESH_TOKEN>",
  "token_type": "Bearer",
  "id_token": "<JWT_ID_TOKEN>",
  "scope": "openid email profile"
}
