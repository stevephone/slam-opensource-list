本仓库是关于开源slam项目汇总
====

#2021年开源SLAM算法整理
----
## 1.Range-MC

>该算法由伯恩大学Cyrill Stachniss团队开源的激光SLAM算法，可用于自动驾驶汽车的激光雷达全局定位，该工作基于蒙特卡罗和粒子滤波来估计移动机器人或自动驾驶汽车的姿态以实现全局定位，传感器模型将当前激光雷达扫描的距离图像还有三角网格渲染的合成距离图像，进行比较跟新粒子权重，该方法简单有效，可以在不同的数据集和环境中使用不同类型的激光雷达扫描，无需微调，并且在动态的室外大范围环境中取得良好的全局定位结果

>>Github地址：https://github.com/PRBonn/range-mcl  [项目地址](https://github.com/PRBonn/range-mcl)

## 2.MULLS
>苏黎世联邦理工学院、禾赛、洛桑联邦理工学院开源的一种高效、低漂移、通用的三维激光雷达SLAM系统。适用于各种场景，各种规格的激光雷达。前端使用双阈值地面滤波和PCA，从每帧中提取地面、柱子等特征，然后利用多尺度线性最小二乘ICP算法，实现了当前帧与局部子地图的配准。对于后端，在存储的历史子图之间进行分层位姿图优化，以减少因航位推算而产生的漂移。

>>Github地址：https://github.com/YuePanEdward/MULLS  [项目地址](https://github.com/YuePanEdward/MULLS)

## 3.LiLi-OM
>德国卡尔斯鲁厄理工学院，开源的紧耦合激光雷达-惯性里程计SLAM算法，它专门用于固态机械激光雷达SLAM。主要特点：

* 针对Livox Horizon的不规则扫描模式量身定做了新的特征提取方法；

* 前端为基于特征的轻量级激光雷达里程计，采用自适应关键帧选取，提供快速的运动估计；

* 后端采用基于关键帧的分层滑动窗口优化，以直接融合IMU和LIDAR测量数据。

>>Github地址：https://github.com/KIT-ISAS/lili-om    [项目地址](https://github.com/KIT-ISAS/lili-om)

## 4.FAST-LIO2
>香港大学张富团队开源的新一代激光雷达惯性里程计FAST-LIO2，该方法可用于自动驾驶、无人机、快速移动的手持设备等场景。有点如下：

* 计算效率高，在大型室外环境中帧率能达到100HZ；

* 鲁棒性高，在宣战度高达1000度/秒的杂乱室外环境中进行可靠的姿态估计；

* 通用性好，使用于多线旋转和固态激光雷达、无人机和手持平台；

* 精度高，能获得更高或与现有方法相当的精度

>>Github地址：https://github.com/hku-mars/FAST_LIO    [项目地址](https://github.com/hku-mars/FAST_LIO)

## 5.LVI-SAM
>麻省理工大佬TixiaoShan继LIO-SAM又开源了lvi-sam,这是一个激光+视觉+惯性的紧耦合多传感器融合的slam系统。用于移动机器人的实时状态估计和建图。主要创新点：

* 通过因子图同时实现多传感器融合、全局优化和回环检测；

* 通过故障检测机制、避免单一子系统故障导致系统不能使用的情况，提高了整个系统鲁棒性；

>>Github地址：https://github.com/TixiaoShan/LVI-SAM    [项目地址](https://github.com/TixiaoShan/LVI-SAM)
