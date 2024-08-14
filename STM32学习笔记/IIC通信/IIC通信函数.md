# IIC通信函数
***
## 接收函数：
~~~C
HAL_I2C_Master_Receive(I2C_HandleTypeDef *hi2c, uint16_t DevAddress, uint8_t *pData, uint16_t Size, uint32_t Timeout)
~~~
第一个参数是**I2C的句柄**
第二个参数是**设备地址**
第三个参数是**接收数据的缓冲区**（指针类型）
第四个参数是**接收数据的长度**
第五个参数是**超时时间**
***
## 发送函数：
~~~C
HAL_I2C_Master_Transmit(I2C_HandleTypeDef *hi2c, uint16_t DevAddress, uint8_t *pData, uint16_t Size, uint32_t Timeout)
~~~
第一个参数是**I2C的句柄**
第二个参数是**设备地址**
第三个参数是**发送数据的缓冲区**（指针类型）
第四个参数是**发送数据的长度**
第五个参数是**超时时间**