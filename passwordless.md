Create key:

```
ssh-keygen
```
Note: Just press enter for all the options

This command will create a public key and a private key under ~/.ssh
public key file will end with .pub. 

To enable the passwordless loging this public key needs to be copied to the remote computer.

copy public key:

```
ssh-copy-id -i ~/.ssh/id_rsa.pub username@serveraddress
```

If 'ssh-copy-id' not installed in your system, you can do copy paste the content of the id_rsa.pub to ~/.ssh/authorized_keys.
scp is another option.
