Usage:

1) Import SQL from sql/oauth.sql

2) Setup database credentials in application/config/database.php

3) Setup .htaccess to remove index.php from the URL

4) Get the access token using:

    POST http://localhost/codeigniter-oauth2-server/resource

    Request patameters in body:
    grant_type     password
    client_id      testclient
    client_secret  testpass
    username       user
    password       pass

5) To access the resource using the access token:

    POST http://localhost/codeigniter-oauth2-server/resource

    Request patameters in body:
    access_token  e7f42c4215e92c9666fa25e6975536ed7b70e80d
