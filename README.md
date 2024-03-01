# Rlogin

A remote authentication and login solution.

This software comes with an authentication server program, and a login program. The authentication server is responsible for handling authentication requests from clients. A client, such as the login program, sends the user's credentials to the server. The server compares these credentials against its /etc/passwd and /etc/shadow database. If the credentials are correct, the server sends the user's information (uid, gid, homedir, shell) to the client, who can use it to authenticate. If not, an "incorrect" response is sent.