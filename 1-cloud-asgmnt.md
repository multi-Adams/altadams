# First Cloud Engineering Assignment via Altadams

Here's how I tackled the assignment:

a. To change to the tests directory using an absolute pathname, I ran:

```bash
cd /home/altschool/tests
```

b. I changed to the tests directory using a relative pathname:

```bash
cd tests
```

c. I created fileA with the text 'Hello A' in the misc directory:

```bash
echo 'Hello A' > /home/altschool/misc/fileA
```

d. I created an empty fileB in the misc directory and populated it with dummy content:

```bash
touch /home/altschool/misc/fileB
echo 'My name is Adams and I am a Cloud engineering student at AltSchool Africa' > /home/altschool/misc/fileB
```

e. I copied contents of fileA into fileC:

```bash
cp /home/altschool/misc/fileA /home/altschool/misc/fileC
```

f. I moved contents of fileB into fileD:

```bash
mv /home/altschool/misc/fileB /home/altschool/misc/fileD
```

g. I created a tar archive called `misc.tar` for the contents of the misc directory:

```bash
tar -cf /home/altschool/misc/misc.tar /home/altschool/misc
```

h. I compressed the tar archive to create a misc.tar.gz file:

```bash
gzip /home/altschool/misc/misc.tar
```

I. I created a user and force the user to change their password upon login with:

```bash
sudo useradd -m -p '*' -e 0 -f 0 akano
```

J. To lock a user's password, I used:

```bash
sudo passwd -l username
```

K. To create a user with no login shell, I ran:

```bash
sudo useradd -s /bin/false amoo
```

L. I edited the sshd_config file (usually located in /etc/ssh/sshd_config) and set to disable password-based authentication for SSH:

```bash
PasswordAuthentication no
```

M. Similarly, I edited the sshd_config file and set to disable root login for SSH:

```bash
PermitRootLogin no
```

...and all done!! See you in the next one! 👋🏾
