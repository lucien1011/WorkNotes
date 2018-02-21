# Short recipe for UF computing 

[Web server for T2 Florida](http://tier2.ihepa.ufl.edu/)
[UF research computing](https://www.rc.ufl.edu)

--------------

#### A full list of ihepa machines
archer, alachua, melrose, newberry, or gainesville.ihepa.ufl.edu

```
ssh -X -Y lucien@newberry.ihepa.ufl.edu
```

--------------

#### Copy files from UF Tier 2 storage
```
gfal-copy gsiftp://cmsio.rc.ufl.edu//cms/data/store/user/klo/<PATH_TO_FILE> file://<PATH_TO_COPY_TO>
tar xzvf heppyOutput_3.tgz
```



