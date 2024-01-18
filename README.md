# LineageOS 20 local_manifests
Lineage OS 20 manifest for Samsung S6 and S6 edge International variants

## Steps to build  
1) Clone Lineage 20 repo and setup your build environment according to the lineage documentation  
2) Clone 7420_patches and follow the instructions to apply them. **THIS IS REQUIRED FOR WORKING BUILDS AND IS MANDATORY**  
3) Follow the general guidance on local_manifests in order to clone all necessary repos  
4) Open the Lineage 20 root folder  
5) source build/envsetup.sh  
6) lunch lineage_[codename]-userdebug  
7) make bacon -j[cpucorecount]  

wait for it to build and flash the zip

