Display replicas configuration:
```
rs.conf()
```
and check replication status:
```
db.printSlaveReplicationInfo()
```
Change SECONDARY to PRIMARY:
on all replicas:
```
rs.freeze(120)
```
to not elect them as PRIMARY.
On PRIMARY:
```
rs.stepDown(120)
```

Check active connections:
```
db.currentOp()
```
Check all connections:
```
db.currentOp(true)
```
summary:
```
db.serverStatus().connections
```
