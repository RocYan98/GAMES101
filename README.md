# GAMES101现代计算机图形学入门 作业
## Assignment0 

![image-20230617195712058](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/eroes6.png)

## Assignment1: Rotation and Projection

![屏幕录制2023-06-19 22.05.30](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/uyn2qd.gif)

## Assignment2: Triangles and Z-buffering

如果直接输出会和参考答案是关于中心对称的![](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/8jpmrs.png)

参考了[闫令琪：GAMES101 现代计算机图形学-作业ASSIGNMENT02解析](https://blog.csdn.net/weixin_39548859/article/details/107092229)和[HW02的疑问](http://games-cn.org/forums/topic/hw2的疑问/#post-6731)后发现这个代码框架使用的是左手坐标系，而课程使用的是右手坐标系，这样会导致结果与参考答案关于原点中心对称。把main.cpp的[57:19]修改为-1，把rasterizer.cpp的第90行改为`vert.z() = -vert.z() * f1 + f2;`就可以得到正确答案。![](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/vikbxp.png)

## Assignment3: Pipeline and Shading

作业3和作业2一样也需要修改坐标系，否则只能看到牛屁股。在实现作业3之前建议先看[作业3更正公告](http://games-cn.org/forums/topic/作业3更正公告/)中的“作业三常见问题集合”。

实现 Normal Shader 后：![image-20230627201458386](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/g3magk.png)

实现 Blinn-Phong 反射模型之后：![image-20230628171630162](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/ckyeqa.png)

实现 Texture 后：![image-20230628173233251](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/57639p.png)

实现 Bump Mapping 后：![image-20230628182343198](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/xnicq0.png)

实现 Displacement Mapping 后：![image-20230628183530834](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/wsxkis.png)

## Assignment4: Bézier Curve

![截屏2023-07-21 16.48.57](http://rocyan.oss-cn-hangzhou.aliyuncs.com/notes/8b9wn6.png)