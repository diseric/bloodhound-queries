# bloodhound-queries

```
MATCH(((u1:User)-[r1:MemberOf*1..]->(g1:Group))) MATCH p2=(u1)-[:Owns*1..]->(c:Computer) RETURN p2
```
