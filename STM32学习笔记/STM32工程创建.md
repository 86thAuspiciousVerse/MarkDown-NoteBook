# 工程创建
## CubeMX内：
1. 配置GPIO
2. SYS/Debug 设定为Serial Wire使用stlink接入
3. 设定project manager ，写名字，设定项目保存路径，Toolchain设定为CubeMX
4. 使用外设的话就进入 project manager/code generator勾选“为每个外设生成独立的.c/.h文件”
5. 去对应的文件夹右键用CLion打开

## CLion内：
1. 一般会自动检测到stm32 project
2. Debug（小虫子）右边，省略号打开
3. 编辑
4. “+”号
5. 选择openOCD下载并运行
6. 选择唯一的可执行文件xxx.elf
7. 选择编译器arm-none-eabi
8. 选择面板文件
9. 面板文件在stm32config文件夹内
10. 进入STM32F103C8TX.ld内
11. ctrl+f查找并替换所有的“READONLY”
12. 下载改为始终
13. 应用确定


## 注意
- 如果设定的时候忘记设定debug，将无法写入程序
- 此时应该将两个跳线帽往下移动，此时可以写入程序
- 写入程序后，将两个跳线帽往上移动，此时才可以运行程序