### Standalone production

```
cmsrel CMSSW_X_Y_Z 
cd CMSSW_X_Y_Z/src
cmsenv
tar -xavf <path of gridpack creation>/wplustest_LO_tarball.tar.xz
bash
./runcmsgrid.sh <NEvents> <RandomSeed> <NumberOfCPUs>
```
