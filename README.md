# mi-UGens

Some *mutable instruments* eurorack modules ported to [SuperCollider](https://supercollider.github.io/)

Thanks to Émilie Gillet for making the original source code available!
https://github.com/pichenettes/eurorack

**Please note, this is NOT a project by [mutable instruments](https://mutable-instruments.net/) !**

Volker Böhm, 2020
https://vboehm.net


##
Updated for linux compilation 4/30/2020 by Steven Noreyko


## Building for linux (Raspberry Pi)

```
# need cmake if you dont already have it
sudo apt-get install cmake

cd ~/
git clone https://github.com/v7b1/mi-UGens.git
git clone https://github.com/supercollider/supercollider.git  
cd supercollider
git submodule update --init
cd ~/mi-UGens

# then cd to directory you want to build

cd MiClouds
mkdir build && cd build
cmake -DSC_PATH=~/supercollider ..
cmake --build . --config Release

```
