**Log in Via ssh with password(Local Server)**

```
Login via SSH with password (LOCAL SERVER)
\$ssh caleb@192.168.1.29
```

**Create folder ,file and install apache**

```
\$mkdir test

\$cd test

\$touch hello.txt

\$sudo apt-get install apache2

**Generate Keys(Local Machine)**

\$ssh-keygen
```

**Add key to server in one command**

```
> cat ~/.ssh/id_rsa.pub | ssh brad@192.168.1.29 "mkdir -p ~/.ssh && chmod 700 ~/.ssh && cat >> ~/.ssh/authorized_keys

This will help you avoid keying in the password while pinging into your server.

```

**Create and copy a file to the server using SCP**

```
touch test.txt $ scp ~/test.txt brad@192.168.1.29:~

```
