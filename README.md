# Satellite-navigation-practice-questions
Some practice questions on satellite navigation

最近学习了一些GPS卫星导航的一些知识，用matlab实现了三道实践题

比较简单，仅供参考，有问题欢迎指出
## 实践内容I : L1频点C/A码信号的并行捕获
- 建议时间： 约3~4h
- 工具：MATLAB
- 内容
    1. 生成信号：信息速率50bps，伪码速率1.023MHz，码长度1023，自行设定中频、多普勒频率和伪码相位偏移，采用 BPSK调制，信噪比为30dB；
    2. 设定积分时间，采用相干或者非相干积分对信号进行捕获；
- 要求
    1. 图示多普勒和伪码的捕获结果；
## 实践内容II : 利用卡尔曼滤波器模拟目标跟踪过程
- 建议时间：约3-4h
- 工具：MATLAB
- 内容
1. 模型建立：初始距离80km，速度8km/s，采样间隔0.5s，其量测模型是目标到传感器的距离，其噪声标准偏差km，该模型的状态向量为距离和他的变化率，在车辆驾驶中的速度噪声标准偏差（均为高斯白噪声），模型总观测时间为20s
2. 根据模型生成真实值和测量值；
3. 根据卡尔曼滤波计算出估计值；
- 要求
    1. 显示距离、速度的真实曲线、测量曲线和滤波曲线；
    2. 显示距离、速度的偏差曲线和RMSE曲线；
    3. 显示距离、速度的卡尔曼增益曲线和协方差曲线；
## 实践内容Ⅲ : 根据星历数据实现卫星位置计算
- 建议时间：约3-4h
- 工具：MATLAB
- 内容
    1. 读取.n星历文件并从中提取出卫星参数；
    2. 根据相应参数计算出卫星位置；   
- 要求
    1. 理解.n文件文件头和数据的含义；
    2. 计算卫星的三维位置；
    3. 链接中给出的数据是GPS的，可自行下载北斗或伽利略的数据计算卫星位置；下载链接可参考：[北斗/GNSS相关数据下载地址合集（未整理完）GAMIT/BERNESE - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/285099374)


## Practice I: Parallel acquisition of L1 C/A code signal
- Recommended duration: About 3 to 4 hours
- Tool: MATLAB
- Content
1. Generated signal: information rate 50bps, pseudo-code rate 1.023MHz, code length 1023, self-set IF frequency, Doppler frequency and pseudo-code phase offset, BPSK modulation, signal-to-noise ratio of 30dB;
2. Set the integration time and capture the signal by coherent or incoherent integration;
- Requirement
1. Figure Doppler and pseudo-code capture results;
## Practice II: Using Kalman filter to simulate target tracking process
- Recommended time: about 3-4h
- Tool: MATLAB
- Content
1. Model establishment: the initial distance is 80km, the speed is 8km/s, the sampling interval is 0.5s, the measurement model is the distance from the target to the sensor, its noise standard deviation km, the state vector of the model is the distance and its rate of change, the speed noise standard deviation in the driving of the vehicle (all are Gaussian white noise), the total observation time of the model is 20s
2. Generate real values and measured values according to the model;
3. Calculate the estimated value according to the Kalman filter;
- Requirement
1. Display the real curve, measurement curve and filter curve of distance and speed;
2. Display deviation curve and RMSE curve of distance and speed;
3. Kalman gain curve and covariance curve showing distance and speed;
## Practice content III: Satellite position calculation based on ephemeris data
- Recommended time: about 3-4h
- Tool: MATLAB
- Content
1. Read the.n ephemeris file and extract satellite parameters from it;
2. Calculate the satellite position according to the corresponding parameters;
- Requirement
1. Understand the meaning of the header and data in an.n file.
2. Calculate the three-dimensional position of the satellite;
3. The data given in the link is GPS, you can download the data of Beidou or Galileo to calculate the satellite position;
