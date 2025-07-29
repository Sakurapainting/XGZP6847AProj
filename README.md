

# XGZP6847AProj压力传感器+串口

# XGZP6847AProj —— STM32压力传感器串口通讯项目

## 项目简介
本项目基于 STM32F103C8T6 单片机，使用 HAL 库驱动 XGZP6847A 压力传感器，并通过串口（UART）与上位机通讯。适用于压力采集、数据传输等嵌入式场景。

## 硬件接线
### 压力传感器 XGZP6847A
1. 不接
2. STM32 3.3V
3. STM32 GND
4. STM32 3.3V
5. STM32 GPIO PA5
6. STM32 GND

### USB转串口模块
1. GND — STM32 GND
2. RX  — STM32 PA9
3. TX  — STM32 PA10

## 环境依赖
- STM32CubeMX
- Keil5 (MDK-ARM)
- STM32F103C8T6 开发板
- XGZP6847A 压力传感器

## 目录结构说明
```
Core/
  Inc/    # 头文件
  Src/    # 源文件
Drivers/  # HAL库及CMSIS
MDK-ARM/  # Keil工程文件
README.md # 项目说明
```

## 开发架构
- 使用 STM32 HAL 库进行外设初始化和数据采集
- 通过 ADC 采集压力传感器数据
- 串口（USART）实现数据发送到上位机

## 部署与编译
1. 使用 STM32CubeMX 生成初始化代码
2. 用 Keil5 打开 MDK-ARM 目录下的工程文件 `.uvprojx`
3. 编译并下载到 STM32F103C8T6 开发板

## 作者
邮箱：you2899047197@163.com

## 版本控制
本项目使用 Git 进行版本管理，详见仓库历史。

## License
本项目采用 MIT License 开源协议，详见 LICENSE 文件。


