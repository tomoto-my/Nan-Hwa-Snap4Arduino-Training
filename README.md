# Nan Hwa Snap4Arduino Training

**Nan Hwa Snap4Arduino Training** 是 **_espSnap_** 项目的配套教程。

它有以下目标

(1) 向用户展示如何在 **Snap4Arduino** 中使用 Snap*!*
(2) 展示在 **Snap4Arduino** 中使用 **_espSnap_** 的简易性
(3) 让用户学习和使用 **_espSnap_** Arduino 板
(4) 让用户通过 **_espSnap_** 学习一些电子基础知识
(5) 让用户将学习体验扩展到 **_espSnap_** 已整合功能的 Arduino 模块


它分为 3 个课程，如下所示：
第一节 : 图块编程 Snap! 简介
第二节 : 图块编程 Snap! + Arduino 结合的基础
第三节 : 结合图块编程 Snap! 与 Arduino 集成模块

本配套教程包含带有示例的解释和说明。



### 第一节 : 图块编程 Snap! 简介
- 第 1 节是关于 **Snap4Arduino** 的 图块编程 Snap*!* 基本介绍
- 它包含关于 Snap*!* 8 个主要类别的章节
    并举例说明了大多数常用块的功能或用途
- 以及关于如何在 **Snap4Arduino** 中创建自定义块以简化块脚本（代码）的章节
- 这使初学者能够对 Snap*!* 有相当的了解
- 并能够开始创建自己的互动故事、游戏和动画

- 有关 Snap*!* 详细说明，请参阅 [**Snap_!_** 参考手册](https://snap.berkeley.edu/snap/help/SnapManual.pdf)。


### 第二节 : 图块编程 Snap! + Arduino 结合的基础
- 第 2 节介绍在 **Snap4Arduino** 中使用 **espSnap_Library** 的基本 Arduino 功能
    基本功能列表如下：
    - 数字输入
    - 数字输出
    - 模拟输入
    - 模拟输出
        - DAC [1]
        - PWM
        - 伺服
        - 音调
- 示例包含详细解释

### 第三节 : 结合图块编程 Snap! 与 Arduino 集成模块
- 第 3 节介绍在 Snap4Arduino 中使用 espSnap_Library 的附加功能


<BR>

---

**Nan Hwa Snap4Arduino Training** is a companion tutorial for the **_espSnap_** project.

It has the following objectives

(1) to show users how to use Snap*!* in **Snap4Arduino**
(2) to demonstrate the ease of using **_espSnap_** in **Snap4Arduino**
(3) to allow users to learn and use the **_espSnap_** Arduino board
(4) to allow users to learn some basics of Electronics via **_espSnap_**
(5) to allow users to extend the learning experience to the Arduino Modules which **_espSnap_** have incorporated the functions


It is organized into 3 sessions as follows :
- Session 1 : **Introduction to Visual Programming Snap!**
- Session 2 : **Basic Functions of Snap! + Arduino**
- Session 3 : **Use Arduino Modules with Snap!**

This companion tutorial contains explanations and instructions with examples.

<BR>

---
### Session 1 : Introduction to Visual Programming Snap!
- It has a section on each of the 8 main categories of Snap*!*
    with example of the function or purpose of most of the commonly used blocks
- plus a section on how to create custom block in **Snap4Arduino** to simplify the block scripts(codes)
- this allows beginners to have a quite understanding of Snap*!*
- and be able to start create their own interactive stories, games and animations

- Refer to [**Snap_!_** Reference Manual](https://snap.berkeley.edu/snap/help/SnapManual.pdf) for detailed explanations on Snap*!*.

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

- examples contained detailed explanations

### Session 3 : Use Arduino Modules with Snap!
- Session 3 allows users to interact with **_espSnap_** to perform the Additional Functions of the **espSnap_Library**

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

- examples contained detailed explanations

<BR>

---
## Import espSnap_Library into Snap4Arduino
Just click on **_File->Imports..._** in Snap4Arduino and navigate to the **espSnap_Library.xml** file and select it

The custom blocks will appear in Snap4Arduino
The custom blocks are currently split into the following 3 categories:
(1) inside the **Arduino** category
(2) **NeoPixel** category
(3) **OLED SSD1306** category

### (1) inside the Arduino category
This portion contains the
- All Basic functions provided by **_espSnap_**
- Additional Module functions provided by **_espSnap_** as follow:
    - DHT22
    - DS18B20
    - HC-SR04
    - Rotary Encoder
    - I2C LCD functions

### (2) NeoPixel category
Various functions to control NeoPixels connected to **_espSnap_**
Maximum number of NeoPixel is limited to 300

### (3) OLED SSD1306 category
Various functions to control OLED SSD1306 connected to **_espSnap_**
connection is via the SCL/SDA pins using I2C protocol
