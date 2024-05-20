# LineageOS 20 local_manifests
Lineage OS 20 manifest for Samsung S6 and S6 edge International variants

## Steps to build  
1) Clone Lineage 20 repo and setup your build environment according to the lineage documentation  
2) Clone 7420_patches (lineage-20 branch) and follow the instructions to apply them. **THIS IS REQUIRED FOR WORKING BUILDS AND IS MANDATORY**  
3) Copy universal7420.xml to {ANDROID_ROOT}/.repo/local_manifests/roomservice.xml - create the folder if it doesnt exist 
4) Return to {ANDROID_ROOT} and repo sync
5) source build/envsetup.sh  
6) lunch lineage_[codename]-userdebug  
7) make bacon -j[cpucorecount]  

Replace codename with the device you are trying to build.
Valid codenames:
- zerofltexx : for the FLAT version of the S6 (G920)
- zeroltexx: for the EDGE version of the S6 (G925)

Replace core count with the number of CPU cores you have.
