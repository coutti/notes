## 1、安装步骤
` conda info`

` conda activate base`

` conda install geos`

` conda install pyproj`

sudo pip install --user git+https://github.com/matplotlib/basemap.git
这一步比较慢，因为克隆下来的文件很大


如果出现从冲突，可以先移除一些包：
`conda remove geos pyproj basemap`

`pip uninstall basemap -y`

`pip uninstall geos -y`

`pip uninstall pyproj -y`


## 2、测试步骤
进入python之后，测试是否安装成功：
``` python
from mpl_toolkits.basemap import Basemap
import matplotlib.pyplot as plt
map = Basemap()
map.drawcoastlines()
plt.show()
```
