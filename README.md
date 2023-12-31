# UART_RX

## 1. Create : New Project
  In windows 11 Machine,  Choose CUBEIDE application and click on it
  
### 1.1 Open CubeIDE
When STM32CubeIDE is started the first time, the Information Center opens.The Information Center enables the user to quickly reach information about the product and how to use it. The Board selector  tabs can be selected at the top of the window. Use the first tab to create a project for a specific device.

![image](https://github.com/DLinIoTedge/Harpy/assets/144312729/b323e9d6-7997-4d5e-a0d4-6fbbdcaecbda)

###  1.2 Choose Board and IC part Number

In Board selector give the Commercial Part Number - NUCLEO-L496ZG-P.select Nucleo-L496ZG-P in the  Board list item.

  ![image](https://github.com/DLinIoTedge/Harpy/assets/144312729/07b08d01-ff1e-4072-9d2c-38b3687d9dec)
  
###  1.3 Create  New Folder and Provide Name
To create a Project, go to [File]>[New]>[C/C++ Project]. This opens the window displayed in the below figure.

![image](https://github.com/DLinIoTedge/Harpy/assets/144312729/d2a434c8-c47f-406b-80bf-3461c94f6807)

### 1.4 Finish
Project folder is created click on next -> finish.

##  2. Resource Allocation

### 2.1 Pin B7 is allocated for LED ( GPIO output pin)
After creating a new project it opens Pinout & Configuration in that select GPIO PB7 pin as LED (GPIO_out) as per the datasheet.
PB7- LED [GPIO_OUT]

### 2.2 UART 3 is allocated ( Asynch mode)
In Pin configuratiuon Click on connectivity select USART 3 as an asynchronous mode as per the data sheet.
PC4 - USART 3_TX [Asynchronous Mode]
PC5 - USART 3_RX

![image](https://github.com/DLinIoTedge/Harpy/assets/144312729/cb3ae49d-d59c-46a8-9699-1d4839253a49)

## 3. Code Generation and Build
Once you created the project and enabled the GPIO (PB7) and UART3 (PC4 and PC5), now we will have the auto generated code.It will open the main.c file in this working space we have to implement our code.
—> In main.c use the printf that will be redirected to the UART3.

## 4.  Connect Target Nucleo Board with UART

Hardware connection - Connect Nucleo-L496ZG-P Board to the PC through USB cable and connect UART to another PC as shown in the figure.

![image](https://github.com/SGyashu/STM32_RX/assets/144312729/da491818-3777-44e3-bde5-784c16c5a2f5)

![image](https://github.com/SGyashu/STM32_RX/assets/144312729/07f2fc81-4895-4f96-8e22-480b42a8638e)




