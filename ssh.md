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

Otherwise you cannot log into the server if it lacks this opensshd
(c)The server must have sshd installed and running or you will not be able
to connect via ssh.


N/B
The sshd config file helps you make security provisions for your server.

ssh config is an important file that can enable you to achieve a couple of things example
disable password login for the root user as well as other security provisions in your servers.

{Example you may disable root/password/login}

```

**_Authentication methods_**

```

ssh caleb@192.168.1.12

(a)via password.

(b)public and private key pair

(c)Host based (stores a list of any known hosts that is
allowed to connect to your machine)

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

Thus the server knows the hosts allowed to connect to it...

{eg i do not want to keep putting the password}

```

**_What about Windows_**

```

(a)ssh has always been  available in windows and mac because they are unix
based systems.

(b)Windows did not support native ssh until very recently .

(Windows 10 now supports native ssh)

(c)On older verisions of windows we  would use what we call putty and putty gen..

Putty gen was used to create the keys.
Putty was used to connect to the server.

(d)git bash and other termninal programmes include the ssh command and other
unix tools.

```
