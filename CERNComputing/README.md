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

### Accessing PSI T3
```
gfal-ls -l root://t3se01.psi.ch:1094//store/user/cheidegg/sea/12/2017-02-24-11-30-00_2lss_bkg/
```
