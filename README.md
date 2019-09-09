# get_pic_address
应用高德地图API获取原图中的地址信息

## 高德地图API 
网站主页：https://lbs.amap.com/

先在《开发支持》--> 《web服务》 --> 《web服务KPI》中获取key，具体操作方法见网站内说明。

## 参数
* img_path ：原图路径
* key ：高德KPI请求URL的参数key。在Location类中__init__修改。

## 函数说明
* transform_GPScoordinate:把图片上的GPS经纬度信息转换为数值型的GPS坐标
* GPS_to_gaodeCoordinate：GPS坐标转高德地图坐标
* get_address：通过高德坐标请求地理位置信息

## Note
必须为带有GPS信息的原图，否则在应用类Location的时候匹配不出GPS坐标信息，报错。




