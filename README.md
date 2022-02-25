# spack_gptune_nersc
## Cori installation 
```
git clone https://github.com/liuyangzhuan/spack_gptune_nersc  
cd spack_gptune_nersc  
module load spack/0.17.0  
cp -r cori_spack-0.17.0/* $SPACK_MYREPO/.  
spack install -v gptune@master~mpispawn%gcc@10.1.0 ^libbsd@0.10.0  
```
## Cori testing
```
allocate a Haswell node  
spack load gptune  
spack test run gptune  
``` 
