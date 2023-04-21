

# README_steeve

in my_path/test_kilosort3/

1. git clone kilosort 

2. git clone https://github.com/kwikteam/npy-matlab.git

3. download small dataset: https://github.com/kwikteam/phy-contrib/blob/master/docs/template-gui.md
    * https://codeload.github.com/kwikteam/phy-data/zip/master

```bash
curl -o data.zip https://codeload.github.com/kwikteam/phy-data/zip/master
unzip data.zip
rm -f data.zip
mv phy-data-master data
```

4. set paths in ../test_kilosort/main_kilosort3.m

5. Setup matlab and run CUDA/mexGPUall.m

```bash
module load unstable hpe-mpi/2.25.hmpt matlab/r2019b
cd CUDA/
matlab -batch mexGPUall # make sure /tmp is cleaned (enough space)
```

