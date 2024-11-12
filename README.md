# Nan Hwa Snap4Arduino Training

## [中文版使用说明]

**Nan Hwa Snap4Arduino Training** 是 **_espSnap_** 项目的配套教程。

该项目的灵感来自于为 **马来西亚曼绒南华独立中学** 学生提供低门槛入门级学习Arduino的工具。

它有以下目标

1. 向用户展示如何在 **Snap4Arduino** 中使用 Snap!
2. 展示在 **Snap4Arduino** 中使用 **_espSnap_** 的简易性
3. 让用户学习和使用 **_espSnap_** ，熟悉 Arduino 的基本功能
4. 同时，在接触和学习 **_espSnap_** 中学习一些电子基础知识
5. 让用户将学习体验扩展到 **_espSnap_** 已整合功能的 Arduino 模块


它分为 3 节课程，如下所示：

- **第一节 : 图块编程 Snap! 简介**
- **第二节 : 图块编程 Snap! + Arduino 结合的基础**
- **第三节 : 结合图块编程 Snap! 与 Arduino 集成模块**

本配套教程包含带有示例的解释和说明。


<BR>

---
### 第一节 : 图块编程 Snap! 简介
第 1 节是关于 **Snap4Arduino** 的图块编程 Snap! 基本介绍

- 它包含关于 Snap! 8 个主要类别的章节<BR>
    并举例说明了大多数常用块的功能或用途
- 以及关于如何在 **Snap4Arduino** 中创建自定义块以简化块脚本（代码）的章节
- 这使初学者能够对 Snap! 有相当的了解
- 并能够开始创建自己的互动故事、游戏和动画
- 示例包含详细解释

- 有关 **Snap!** 更多的详细说明，请参阅 [Run Snap!](https://snap.berkeley.edu/) 的 [**Snap!** 参考手册](https://snap.berkeley.edu/snap/help/SnapManual.pdf)。


<BR>

### 第二节 : 图块编程 Snap! + Arduino 结合的基础
第 2 节指导用户使用 **espSnap_Library** 与 **_espSnap_** 进行交流，执行Arduino的以下基本功能
- 基本功能列表如下 :

    |        基本功能列表        |
    |:------------------------:|
    | 数字输入 |
    | 数字输出 |
    | 模拟输入 |
    | 模拟输出 |
    | - DAC [1] |
    | - PWM |
    | - 伺服 |
    | - 音调 |

    ##### 注 [1] ：模拟输出 - DAC 仅适用于 ESP32

- 示例包含详基本 Arduino 功能细解释, 包括
    - 基本 Arduino 功能
    - 一些电子基础知识


<BR>

### 第三节 : 结合图块编程 Snap! 与 Arduino 集成模块
第 3 节介绍在 **Snap4Arduino** 中使用 **espSnap_Library** 的附加功能

- 附加功能列表如下 :

    | 附加功能       | Arduino 部件             |
    |:--------------|:------------------------|
    | I2C OLED | I2C OLED SSD1306 128x64 |
    | I2C LCD | I2C LCD 16x2 |
    | 超声波距离传感器 | HC-SR04 |
    | 温度/湿度传感器 | DTH22 |
    | 温度传感器 | DS18B20 |
    | NeoPixel | WS2812B |
    | LDR 光传感器 | KY-018 |
    | 旋转编码器 | EC11 / KY-040 |
    | 雨量传感器模块 | YL-83 |

- 示例包含详细解释, 包括
    - Arduino 集成模块功能
    - 一些电子基础知识
    - 与模块相关的技术信息


<BR>

---
# 下载 Nan Hwa Snap4Arduino Training

下载最新版本的 ***[Nan_Hwa_Snap4Arduino_Training.zip](https://github.com/tomoto-my/Nan-Hwa-Snap4Arduino-Training/archive/refs/heads/main.zip)*** 后解压压缩包

培训材料位于文件夹 **_Nan_Hwa_SnapSnap4Arduino_Training_** 内

培训材料包括 3 个培训课程的 **_pdf_** 文件和
- **Snap4Arduino** 的示例文件
- 用于课程第 2 节和课程第 3 节的 Arduino 布线、元件和模块连接电路图

<BR>

---
## 将 espSnap_Library 导入 Snap4Arduino
只需在 **Snap4Arduino** 中单击 **_File->Imports..._**，然后导航到 **espSnap_Library.xml** 文件并选择它

自定义块将出现在 **Snap4Arduino** 中

自定义块目前分为以下 3 个类别：

1. 在 **Arduino** 类别内
2. **NeoPixel** 类别
3. **OLED SSD1306** 类别

<BR>

#### (1) 在 Arduino 类别内
- 此部分包含 **_espSnap_** 提供的所有基本功能
- 和下例部分 **_espSnap_** 提供的附加模块功能：

    | 附加功能       | Arduino 部件             |
    |:--------------|:------------------------|
    | 超声波距离传感器 | HC-SR04 |
    | 温度/湿度传感器 | DTH22 |
    | 温度传感器 | DS18B20 |
    | 旋转编码器 | EC11 / KY-040 |
    | I2C LCD | I2C LCD 16x2 |

#### (2) NeoPixel 类别
- 用于控制连接到 **_espSnap_** 的 NeoPixel 的各种功能
- NeoPixel 的最大数量限制为300

    | 附加功能       | Arduino 部件             |
    |:--------------|:------------------------|
    | NeoPixel | WS2812B |

#### (3) OLED SSD1306 类别
- 用于控制连接到 **_espSnap_** 的 OLED SSD1306 的各种功能
- 连接通过 SCL/SDA 引脚使用 I2C 协议进行

    | 附加功能       | Arduino 部件             |
    |:--------------|:------------------------|
    | I2C OLED | I2C OLED SSD1306 128x64 |


<BR>

---
## _espSnap_

连接 **Snap4Arduino** 和 ESP32/ESP8266 Arduino 板的 Http 服务器

**_espSnap_** 可在以下网址获取：

[**https://github.com/tomoto-my/espSnap**](https://github.com/tomoto-my/espSnap)



<BR><BR>

---
# Nan Hwa Snap4Arduino Training

## [English Version Instructions]

**Nan Hwa Snap4Arduino Training** is a companion tutorial for the **_espSnap_** project.

This project has been inspired by the objective to provide a low barrier entry level learning tool for Arduino for **Nan Hwa High School** students in Perak, Malaysia.

It has the following objectives

1. to show users how to use Snap! in **Snap4Arduino**
2. to demonstrate the ease of using **_espSnap_** in **Snap4Arduino**
3. to allow users to learn and use **_espSnap_** and become familiarise with basic functions of Arduino
4. at the same time, thru using of **_espSnap_**, to understand and learn some basics of Electronics
5. to allow users to extend the learning experience to the Arduino Modules which **_espSnap_** have incorporated the functions


It is organized into 3 sessions as follows :
- **Session 1 : Introduction to Visual Programming Snap!**
- **Session 2 : Basic Functions of Snap! + Arduino**
- **Session 3 : Use Arduino Modules with Snap!**

This companion tutorial contains explanations and instructions with examples.

<BR>

---
### Session 1 : Introduction to Visual Programming Snap!
- It has a section on each of the 8 main categories of Snap!
    with example of the function or purpose of most of the commonly used blocks
- plus a section on how to create custom block in **Snap4Arduino** to simplify the block scripts(codes)
- this allows beginners to have a quite understanding of Snap!
- and be able to start create their own interactive stories, games and animations
- examples contained detailed explanations

- Refer to [**Snap!** Reference Manual](https://snap.berkeley.edu/snap/help/SnapManual.pdf) for detailed explanations on Snap!.

<BR>

### Session 2 : Basic Functions of Snap! + Arduino
- Session 2 allows users to interact with **_espSnap_** to perform the following Basic functions of Arduino using the **espSnap_Library**

    | Basic Arduino Functions  |
    |:------------------------:|
    | Digital Input            |
    | Digital Output           |
    | Analog Input             |
    | Analog Output            |
    |   - DAC <sup>[1]</sup>   |
    |   - PWM                  |
    |   - Servo                |
    |   - Tone                 |

    ###### Note [1] : Analog Output - DAC is only available on ESP32

- examples contained detailed explanations on :
    - basic Arduino Functions
    - basic guides on Electronics

<BR>

### Session 3 : Use Arduino Modules with Snap!
- Session 3 allows users to interact with **_espSnap_** to perform the Additional Functions of the **espSnap_Library**
    Following is a list of functions for the modules which **_espSnap_** had incorporated

    | Additional Functions        | Arduino Parts           |
    |:----------------------------|:------------------------|
    | I2C OLED                    | I2C OLED SSD1306 128x64 |
    | I2C LCD                     | I2C LCD 16x2            |
    | Ultrasonic Distance Sensor  | HC-SR04                 |
    | Temperature/Humidity Sensor | DTH22                   |
    | Temperature Sensor          | DS18B20                 |
    | NeoPixel                    | WS2812B                 |
    | LDR Light Sensor            | KY-018                  |
    | Rotary Encoder              | EC11 / KY-040           |
    | Rain Sensor Module          | YL-83                   |

- examples contained detailed explanations on :
    - Arduino Modules
    - basic guides on Electronics
    - technical info related to the modules

<BR>

---
# Download Nan Hwa Snap4Arduino Training

Download the latest version of ***[Nan_Hwa_Snap4Arduino_Training.zip](https://github.com/tomoto-my/Nan-Hwa-Snap4Arduino-Training/archive/refs/heads/main.zip)*** and extract it.

Training material is under the folder **_Nan_Hwa_SnapSnap4Arduino_Training_**

It includes **_pdf_** file for the 3 Training Sessions and
- Examples files for **Snap4Arduino**
- Circuit diagram for Arduino wiring, component and module connection for Session 2 and 3

<BR>

---
## Import espSnap_Library into Snap4Arduino
Just click on **_File->Imports..._** in **Snap4Arduino** and navigate to the **espSnap_Library.xml** file and select it

The custom blocks will appear in **Snap4Arduino**

The custom blocks are currently split into the following 3 categories:
1. inside the **Arduino** category
2. **NeoPixel** category
3. **OLED SSD1306** category

<BR>

#### (1) inside the Arduino category
- This portion contains the **Basic Arduino Functions** provided by **_espSnap_**
- and some of the **Additional Functions** provided by **_espSnap_** as follow:

    | Additional Functions        | Arduino Parts           |
    |:----------------------------|:------------------------|
    | Temperature/Humidity Sensor | DTH22                   |
    | Temperature Sensor          | DS18B20                 |
    | Ultrasonic Distance Sensor  | HC-SR04                 |
    | Rotary Encoder              | EC11 / KY-040           |
    | I2C LCD                     | I2C LCD 16x2            |


#### (2) NeoPixel category
- Various functions to control NeoPixels connected to **_espSnap_**
- Maximum number of NeoPixel is limited to 300

    | Additional Functions        | Arduino Parts           |
    |:----------------------------|:------------------------|
    | NeoPixel                    | WS2812B                 |


#### (3) OLED SSD1306 category
- Various functions to control OLED SSD1306 connected to **_espSnap_**
- connection is via the SCL/SDA pins using I2C protocol

    | Additional Functions        | Arduino Parts           |
    |:----------------------------|:------------------------|
    | I2C OLED                    | I2C OLED SSD1306 128x64 |


<BR>

---
## _espSnap_

## A Http Server bridging Snap4Arduino and ESP32/ESP8266 Arduino boards

**_espSnap_** is available at :

[**https://github.com/tomoto-my/espSnap**](https://github.com/tomoto-my/espSnap)
