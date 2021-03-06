
.. _olivetti_faces:

Olivetti 脸部数据集
========================================

该数据集包含 1992年4月至1994年4月在AT＆T实验室剑桥采集的一组面部图像。
该 :func:`sklearn.datasets.fetch_olivetti_faces` 函数是从AT＆T下载
数据存档的数据获取/缓存函数。

.. _面部图像: http://www.cl.cam.ac.uk/research/dtg/attarchive/facedatabase.html

如原网站所述：
    有四十个不同的个体，每个个体有十张不同的图片。对于某些个体，图像在不同时间拍摄并且改变
    照明和面部表情(睁开/闭上眼睛， 微小/不微笑)和面部细节(戴眼镜/不带眼镜)。所有的图像采用
    黑色均匀的背景，个体处于直立的正面位置。(容许一定的侧移)

图像被量化为256个的灰度级并以8位无符号整数的形式存储；加载器将这些无符号整数转换为[0,1]之间
的浮点值，这样能方面很多算法的使用。

该数据库的"目标"一个是从0到39的整数，代表着图中人物的身份。然而，由于每一类只有十个样例，从
无监督学习或半监督学习的角度来看，这个相对较小的数据集更加有趣。

原始的数据集由92 x 112大小的图像组成，然而这里提供的版本由64 x 64大小的图像组成。

当使用这些图像时， 请致谢AT&T剑桥实验室。