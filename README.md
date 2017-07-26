Usage:

- Import SQL from sql/oauth.sql
- Setup database credentials in application/config/database.php
- Setup .htaccess to remove index.php from the URL

1) Get the access token using:

POST http://localhost/codeigniter-oauth2-server/resource

Request patameters in body:
grant_type     password
client_id      testclient
client_secret  testpass
username       user
password       pass

2) To access the resource using the access token:

POST http://localhost/codeigniter-oauth2-server/resource

Request patameters in body:
access_token  e7f42c4215e92c9666fa25e6975536ed7b70e80d