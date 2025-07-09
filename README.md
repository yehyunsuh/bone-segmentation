**THIS REPO IS NOT MAINTAINED. IF YOU FIND AN ISSUE, PLEASE CREATE A PULL REQUEST SO OTHERS CAN BENEFIT FROM THE FIX.**

Source code behind the paper [Fully automatic and fast segmentation of the femur bone](http://ieeexplore.ieee.org/document/5872823/), 
presented in [ISBI Conference](http://biomedicalimaging.org/) in 2011. 

The repo also contains: 

- the paper 
- the accompanying master thesis with more details about the approach
- sample of 3D CT data

The code was developed in 2010. 

- Linux
```
git clone https://github.com/yehyunsuh/bone-segmentation.git
mkdir tmp
mkdir output
cd bone-segmentation/
cd src/proposed-method/
mkdir build
cd build/
sudo apt install cmake
sudo apt update
sudo apt install libinsighttoolkit4-dev
cmake ../src
make
./SegmentBoneFromCT ../../../sample-volumes/001-CT.nii ../../../tmp ../../../output/001-CT.nii
```
