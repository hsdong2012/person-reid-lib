# person-reid-lib

The pytorch-based lightweight library of person re-identification.

#### Config

Install

```
pip install numpy h5py lmdb
pip install visdom  # Optional. If you don't need a web presentation, don't install it.
```
Install [pytorch and torchvision](https://pytorch.org/)


Indicates the folder of the original files and where the unzipped file is placed
```
# person-reid-lib/lib/utils/manager.py
self._device_dict = xxxx
```


#### Optical Flow

Install opencv
```
pip install opencv-contrib-python
```

Config
```
# person-reid-lib/lib/dataset/utils.py
DataStoreManager.store_optical_flow = True  # if you want to use optical flow, enable it.

# person-reid-lib/tasks/taskname/solver.py
Solver.use_flow = True
```

#### How to run:
```
cd person-reid-lib_folder
sh script/server_0.sh     
```

#### Dataset

Image: VIPeR, Market1501, CUHK03, CUHK01, DukeMTMCreID, GRID,

Video : iLIDS-VID, PRID-2011, LPW, MARS, DukeMTMC-VideoReID


#### Related person ReID projects:

[deep person reid](https://github.com/KaiyangZhou/deep-person-reid)

[MARS-evaluation](https://github.com/liangzheng06/MARS-evaluation)
