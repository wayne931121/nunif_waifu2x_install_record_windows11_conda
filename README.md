# nunif_waifu2x_install_record_windows11_conda

## First create conda env

## Second install pytorch
https://youtu.be/dK8fL2-3SQ8?si=kNDvADz-PFKsy9Vb

## Third Clone and Run and Finish
https://github.com/nagadomi/waifu2x<br>
https://github.com/nagadomi/nunif
```
#I have create the env with conda before, and I arealdy installed PyTorch with CUDA 12.1
#I download zip from https://github.com/nagadomi/nunif and extract to "C:\...\nunif-master\nunif-master"
#the "C:\...\nunif-master\nunif-master" has "waifu2x/download_models.py"
#the r.txt is combine and modify from 
  1. https://github.com/nagadomi/nunif/blob/master/requirements-gui.txt
  2. https://github.com/nagadomi/nunif/blob/master/requirements-gui.txt

conda activate C://ai

pip install --upgrade --no-cache-dir -r r.txt

cd "C:\...\nunif-master\nunif-master"

set KMP_DUPLICATE_LIB_OK=TRUE

python -m waifu2x.download_models

python -m waifu2x.web.webgen

python -m iw3.download_models

pip install -U wxPython

Ok, you done! Start Run waifu2x!

python -m waifu2x.gui

python -m waifu2x.web --no-size-limit --cache-ttl 120

python -m iw3.gui
```
