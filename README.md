
# PIT By jsPsych 实验设计说明文档


## 目录 
- [一、实验简介](#一、实验简介) 
- [二、实验内容](#二、实验内容) 
- [三、操作步骤](#三、操作步骤)
- [四、获得实验数据](#四、获得实验数据) 
- [五、特点](#五、特点)
- [六、参考文献](#五、参考文献)


## 一、实验简介

本实验旨在通过一系列的视觉刺激和用户反馈来评估参与者的反应速度和准确性。本实验范式参考自文献 **(Algermissen等, 2024)**。实验包括两部分：第一部分是主要的实验任务，第二部分是迁移任务。实验结束后，系统将生成一个包含实验数据的CSV文件，供后续分析使用。

![(Algermissen等, 2024)](/sources/reference.png)

## 二、实验内容

1.  **个人信息录入**
    
    -   参与者需要填写编号、姓名、性别、年龄、手机号和学历等基本信息。
2.  **实验指导**
    
    -   在实验开始前，参与者将看到一系列指导图片，说明实验的规则和操作方法。
3.  **主要实验任务**
    
    -   实验包含若干个刺激试次，每个试次由三个阶段组成：
        -   **刺激呈现**：显示一个图像，参与者需要在限定时间内作出反应（按左键或右键）。
        -   **注视点**：显示一个注视点图像，作为间隔。
        -   **反馈**：根据参与者的反应，给出相应的反馈图像和积分。
4.  **休息阶段**
    
    -   实验中途会有一个休息阶段，参与者可以选择休息的时间长度（10秒、30秒、1分钟、1分30秒或2分钟）。
5.  **迁移任务**
    
    -   实验结束后，会进行迁移任务，显示四个图片，参与者需要按上键或下键进行选择。
6.  **最终积分显示**
    
    -   实验结束后，系统会显示参与者的最终积分。

## 三、操作步骤

### 1. 初始化实验

在浏览器中打开包含实验代码的HTML文件，系统将自动进入全屏模式，并显示实验指导信息。

### 2. 录入个人信息

根据提示填写编号、姓名、性别、年龄、手机号和学历等基本信息，然后点击“完成”按钮继续。

### 3. 阅读实验指导

阅读实验指导图片，了解实验规则和操作方法。阅读完毕后，按“继续”按钮开始实验。

### 4. 进行主要实验任务

按照以下步骤进行每个试次：

-   观看刺激图像并在限定时间内作出反应。
-   观看注视点图像，作为间隔。
-   接收反馈图像和积分更新。

目前实验共设计2个block，每个block包含40个trial，可根据需要修改。

### 5. 休息阶段

在提示休息时，选择想要休息的时间长度，然后按“继续”按钮开始休息。倒计时结束后，按任意键继续实验。

### 6. 迁移任务

观看迁移任务图片并按上键或下键进行选择。

### 7. 查看最终积分

实验结束后，系统将显示最终积分，并生成实验数据的CSV文件。

### 8. 退出全屏模式

实验结束后，系统将自动退出全屏模式，鼠标指针重新出现。

## 四、获得实验结果

实验结束后，系统会自动下载实验数据的CSV文件，文件名为参与者的编号。文件包含所有的实验数据，供后续分析使用。

## 五、特点
|特点| 介绍 |
|--|--|
| 全屏 | 在实验开始进入全屏模式，结束后退出全屏，避免实验过程干扰 |
| 鼠标 | 在不需要鼠标时，将鼠标隐藏，避免鼠标影响被试判断 |
| 倒计时 | 在中间休息时，用倒计时告知被试剩余时间 |
| 平衡 | 在不同的block，会将trial顺序打乱，以进行平衡 |
| flexbox | 运用了flexbox，实现响应式布局，适应不同设备 |
| 插件丰富 | 本实验中运用了许多jsPsych插件，如问卷，引导语，全屏，按键反应等 |
| 数据 | 在实验结束，会自动将实验数据以csv格式下载，并用被试编号命名，以供后续分析 |

## 六、参考文献

> Algermissen, J., Swart, J. C., Scheeringa, R., Cools, R., & Den Ouden, H. E. M. (2024). Prefrontal signals precede striatal signals for biased credit assignment in motivational learning biases. _Nature Communications_, _15_(1), 19. [https://doi.org/10.1038/s41467-023-44632-x](https://doi.org/10.1038/s41467-023-44632-x)
