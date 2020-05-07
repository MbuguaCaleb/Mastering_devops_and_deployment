**SSH**

```
(a)Stands for secure shell.

(b)It is a protocol to communicate with other computers.Similar to (http, https,ftp etc)

(c)Do just anything on the remote computer.

(d)Its biggest adavantage is that all of its traffic is encrypted.

{There are other programmes like telnet.The disadvantage with telnet is that it is not encrypted}

(e)It is used mostly in the terminal/commandline.

however there are programmes that allow you to use it like a gui.example winscp and ftp(secure ftp) eg filezilla


```

**Client/Server Communication**

```
(a)ssh is the client


(b)The server you are logging into must have SSHD(Open SSH Daemon)

(c)The server must have sshd installed and running or you will not be able
to connect via ssh.


N/B
The sshd config file helps you make security provisions for your server.

{Example you may disable root/password/login}

```

**_Authentication methods_**

```

ssh caleb@192.168.1.12


(a)via password.

(b)public and private key pair

(c)Host based

Creating a list of known hosts
The file stores any hosts that allowed to login to the machine.

```

**_Generating Keys_**

```

ssh-keygen

(a)~/.ssh/id_rsa(Private Key)

(b)~/.ssh/id_rsa.pub(Public Key)

(c)public key is the one that is transferred to the remote computer.
Public key goes into the server "authorized keys file "

```

**_What about Windows_**

```
It is worthwhile noting that linux and Mac are unix based sytems , thus ssh is easily supported.

How about windows??

(a)Windows 1-


```
