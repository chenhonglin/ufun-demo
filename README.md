#ufun_demo  

在之前板卡测试程序的基础上加入了一些演示功能.    

**demo 功能大致有:**   

- 触摸按键: 按下后背面白色 LED3 会亮, 长按长亮.  
- CH340: ISP以及串口转 USB 功能. 实现串口输出打印.  
- 三轴加速度计: 将三轴的值使用 TIM2 PMW 控制 RGB LED颜色.
- 蜂鸣器: SD 卡插拔会有提示音, 开机会响几秒.
- TIM4 PWM: CH3 CH4 输出两路PWM。
- ADC: 将TIM4 的CH3 CH4 两路PWM经过运放电路作为ADC的输入。
- TIM2 PMW: CH1 CH2 CH3控制 RGB 呼吸效果. 
- SD卡: 读取 SD 卡信息. 插拔识别. 
- RTC: 输出当前日期
- mini PCI-e(IO口测试) 所有IO都有方波输出。

在没有使用 rt-thread 正式开发之前, 希望大家多多贡献自己的代码和想法.    

加入到项目中来.  demo 程序一定会成为以后裸奔或者 RTOS 版本的基础.   

工程直接 clone 下来就可以在 Project 目录内找到 .uvproj(keil MDK 4.x 打开), .uvprojx(keil 5.x 打开).   

我们的版本已经约定使用 KEIL MDK5.15 版本. 其他版本可能会遇到各种问题, 可以发 issues 给我们. 一起 fix.   

加油!  
