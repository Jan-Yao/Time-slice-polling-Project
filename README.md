# 时间片轮询项目
声明：自用时间片轮询项目（只用于学习和改良，不用于任何商业用途）

  1.包含大多数外设（按键扫描、串口通讯、I2C、PWM、定时器、ADC、内部Flash）
  
  2.I2C是使用IO口做的模拟I2C,可能需要微调Sensor_I2CDelay()的时间，以配合不同的从机和使用环境，有条件的可以使用硬件I2C
  
  3.项目内任务装载，未加入watchdog功能，有需要的小伙伴，可以自行添加
  
  4.外设基本实行模块化，一种外设用一个.c和.h搞定，功能函数也写在里面，有需要的小伙伴可以自行更改；但是有些功能由于嵌套，跳转较多，可能看起来有点乱，请谅解
  
  5.有串口和上位机通讯的调试功能，有兴趣的，可自行扩展
  
  6.初次尝试这样的程序，可能逻辑有些地方欠佳，程序有地方有问题，望见谅，欢迎讨论
  
  7.重要：此程序定时中断为25us，建议自用的时候，修改下定时时间（将定时时间改长点），防止中断时间过短，导致的死机现象
  
  8.重要：由于之前公司的项目，所以为了以防扯皮，请大家无视其中提到的公司和产品信息
  
  非常感谢！谢谢！
