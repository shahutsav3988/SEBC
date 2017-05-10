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
