Create Database

```
/usr/sbin/kdb5_util create -s
Loading random data
Initializing database '/var/kerberos/krb5kdc/principal' for realm 'SHAHUTSAV3988.COM',
master key name 'K/M@SHAHUTSAV3988.COM'
You will be prompted for the database Master Password.
It is important that you NOT FORGET this password.
Enter KDC database master key: 
Re-enter KDC database master key to verify: 

```

Add Principal

```
addprinc cloudera-scm@SHAHUTSAV3988.COM
```

Add Policies

```
kadmin.local
kadmin.local:  addpol admin
kadmin.local:  addpol users
kadmin.local:  addpol hosts
```

Kinit commands used to authenticate shahutsav3988 user

```

kinit shahutsav3988
Password for shahutsav3988@SHAHUTSAV3988.COM: 
[root@ip-172-31-1-170 ec2-user]

klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: shahutsav3988@SHAHUTSAV3988.COM

Valid starting     Expires            Service principal
05/10/17 22:14:09  05/11/17 22:14:09  krbtgt/SHAHUTSAV3988.COM@SHAHUTSAV3988.COM
renew until 05/17/17 22:14:09
```
