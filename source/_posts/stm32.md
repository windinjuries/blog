## stm32
## 中断
- 复位
- NMI
- hard fault  
....
- PendSV
- Systick


## 外设
### CAN
[CAN总线协议](https://blog.csdn.net/qq_35057766/article/details/135580884)  
[CAN总线协议](https://blog.csdn.net/MANONGDKY/article/details/143571413)


### SPI
- 硬件接口
 - 四线制： CS SCK MISO MOSI；
 - 输出引脚推挽输出，输入浮空输入或者上拉；
 - 没有应答机制，没有总线仲裁；
 - 主从机都有移位寄存器，当产生一个时钟信号，双方发送一位数据（MSB）
- 信号时序
 - 起始信号：CS拉低
 - 终止信号：CS拉高
 - 极性相位（极性0：空闲为低电平，相位0：第一个边沿移入数据（采样），第二个边沿移出数据）；
 - 信号频率 （stm32f1xx 72MHZ）
- 传输协议
 指令码（0x06）+ 数据
