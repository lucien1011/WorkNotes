### Workbook
[NanoAOD](https://twiki.cern.ch/twiki/bin/view/CMSPublic/WorkBookNanoAOD)

[scram](https://twiki.cern.ch/twiki/bin/view/CMSPublic/SWGuideScram)

### Collection of xrootd path
```
root://cms-xrd-global.cern.ch//store/PATH_TO_FILE
```

### Check xrd access rate
```
xrdcp -d 1 -f root://cms-xrd-global.cern.ch//store/PATH_TO_FILE /dev/null
```

### crab

To start, source crab:
```
source /cvmfs/cms.cern.ch/crab3/crab.sh
```

### Update grid certificate
```
voms-proxy-init --voms cms --valid 168:00
```
