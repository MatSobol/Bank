# Basic bank website

### How to start

you need to write following commands to start website:
```
git clone https://github.com/MatSobol/Bank.git
cd Bank
sudo docker-compose build
sudo docker-compose up
```
If you want password recovery and receive error notification to function you need to give email and password in here:

![image](https://github.com/Mateusz3124/OchronaFixed/assets/95550799/4d10e6a9-1e7d-439a-81ec-9a7d69675aaf)

and set up proper email for accounts in here:

![image](https://github.com/MatSobol/Bank/assets/139177376/1950577b-974a-4314-bad8-9b823ed6c3b4)


to get password from gmail for smtp you need to follow this tutorial:

https://support.google.com/mail/answer/185833?hl=en

tutorial on how to install docker-compose:

https://docs.docker.com/compose/install/

### What i use:
- Nginx with https protocol
- MySql for database
- To encrypt data: aes gcm
- For passwords: argon2
- For general hashes: blake2
- For session: flask session
- For CSRF: flask_wtf

### Accounts for login:

first:

- authentication id: 12345678
- password: aA1!b4B1FG

second:

- authentication id: 87654321
- password: aA1!b4B1FG

### How it looks

Firstly you write your authentication id

![image](https://github.com/Mateusz3124/OchronaFixed/assets/95550799/c8c7c100-e28c-4be0-b030-afb807f7e677)

The minimum size of password is 10 so it only displays 11 blocks where black blocks are empty letters of password

![image](https://github.com/Mateusz3124/OchronaFixed/assets/95550799/7b565b61-cb4e-41f9-8eb3-dd65ff556dbd)

If the password is longer it will dynamically add blocks

![image](https://github.com/Mateusz3124/OchronaFixed/assets/95550799/4899fb91-b3af-47b4-8a9a-4d457a788105)

After login you can see main page of bank. For example:

![image](https://github.com/Mateusz3124/OchronaFixed/assets/95550799/c4beb18f-5974-4456-b0d5-a16aa22e2c56)



