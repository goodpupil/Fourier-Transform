# Fourier-Transform
主要为"离散傅里叶变换(DFT)与卷积(conv)"相关matlab和python程序

说明1：DFT程序中读取外部txt数据文件，格式只有一个要求：**每行数据个数一致**。       

说明2：二维卷积只有一个要求：二维数据矩阵尺寸 **>** 卷积核尺寸(边长最好为奇数)。

# 时间：2019.3.10
新增程序如下：
- 卷积的手动实现(文件名：convolution.m)   
- 例题1——离散函数信号的**DFT**处理，用matlab自带程序和手动实现各一个(文件名：cx1.m与cx1_sx.m);   
- 例题2——原始时域信号与**DFT+IDFT**变换后的时域信号对比，用matlab自带程序和手动实现各一个(文件名：cx2.m与cx2_sx.m);      
- 例题3——频率域的**滤波**操作，并在频域滤波后转换回时域，用matlab自带程序和手动实现各一个(文件名：cx3.m与cx3_sx.m);
- 对原始的循环卷积程序(cyclic_convolution.m)稍微修改，加上用matlab自动语句直接实现的功能;
- 相关说明参考：[一维卷积与一维离散傅里叶变换](https://www.jianshu.com/nb/35397386)。


# 时间：2019.03.23
新增程序如下：
- 二维卷积的手动实现，并用简单的二维矩阵进行测试(文件名：juanji1_2d.m与juanji2_2d.m);
- 二维卷积对图像的处理：用多种卷积核实现不同的图像处理效果(文件名：juanji3_2d.m);
- 二维卷积对图像做滤波：针对"**高斯噪声和椒盐噪声**"做"**中值滤波和均值滤波**"(文件名：noise_mean.m与noise_midval.m);
- 二维反卷积实现(文件名：fjuanji1_2d.m与kz1.m);
- 二维离散傅里叶正变换与逆变换的手动实现(文件名：mydft2.m与myidft2.m);
- 二维离散傅里叶变换后"**频振图中心化**"的手动实现(文件名：center_fft2.m);
- 在二维离散傅里叶变换后的"**频域**"内做"**巴特沃斯低通滤波**"效果(文件名：origin_lowpass_fft2.m);
- 对加了"高斯噪声/椒盐噪声"的二维图像矩阵进行频域滤波(文件名：noise_lowpass_fft2.m与noise_compare.m)。
- 另外，上面很多程序中用到了"**zxc.jpg**"图片，也放了进去方便直接测试程序(文件名：zxc.jpg);
- 相关说明参考：[二维卷积与二维离散傅里叶变换](https://www.jianshu.com/nb/35397386)。


# 时间：2019.04.20
新增程序如下：
- 一维信号小波多级分解与重构/恢复原始信号的手动实现(文件名：xb1d_basic.m与xb1d_recover.m)；
- 一维信号相关matlab自带函数的使用(文件名：oned_process1.m与oned_process2.m)；
- 小波应用1：利用小波多级分解辨识信号中的间断点(文件名：Identify_breakpoint.m)；
- 小波应用2：利用小波和短时傅里叶变换做**时频分析**，研究**时变信号**中**频率随时间**的变化情况(文件名：tfrstft.m与time_freq_analy.m)；
- 小波应用3：小波变换去噪(文件名：wden_qz.m与wdencmp_qz.m)；
- 小波应用4：实际地震数据的时频分析，并绘制等值线图、mesh2d、mesh3d图像(文件名：shiji.m；数据名：shuju.xlsx)；
- 相关参考说明：[小波变换](https://www.jianshu.com/nb/35397386)。     
**注意：时频分析应用时，各个函数都要配上tfrstft.m函数(放在一起)，它里面有一些时频变换的基础功能。**


# 时间：2019.04.25
新增程序如下：
- 地球物理专用的τp变换程序(文件名：tp.m)；
- 相关说明参考：[τp变换](https://www.jianshu.com/p/4439a1cb5c35)。


# 时间：2019.04.28
新增程序如下：
- 一维离散希尔伯特变换手动实现(文件名：Hilbert.m)；
- 根据离散希尔伯特变换得到信号的**3瞬属性**：瞬时振幅/包络、瞬时相位、瞬时频率(文件名：HT3S.m)；
- 相关说明参考：[离散希尔伯特变换](https://www.jianshu.com/p/b591d95ae80b)。


# 时间：2019.05.16
新增程序如下：
- 希尔伯特-黄变换手动实现以及时频分析(文件夹名：HHT1);
- 用自带工具包的函数完成希尔伯特-黄变换与时频分析，并配备更高级的ceemdan分解方式(文件名名：HHT2)；(**推荐**)
- 相关说明参考：[希尔伯特-黄变换](https://www.jianshu.com/p/3363abb64f32)。
