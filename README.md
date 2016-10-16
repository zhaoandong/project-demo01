## 运行流程
### 1、在textarea输入
### 2、执行

## 大概算法
### 1、初始化价格
#### weekdayObj 和 weekendObj 是一个对象，是将每个小时的价格用对象来表示，周末和平时的价格做了区分
### 2、isWeekend 函数
#### isWeekend函数判断日期中是否是周末，从而可以知道匹配对应的价格对象
### 3、conventTime函数
#### conventTime函数将输入的15:00~17:00 转换为标准格式，并输出开始时间和持续时间的长度，方便其他函数调用
### 4、courtCount 函数
#### 因为有固定的算法计算定多少个场地，所以就写了这个函数，传入一个人数，会返回一个定的场地数
### 5、totalPrice 函数
#### 通过传入类似2016-06-07 15:00~17:00 12的值，来计算出花费和收入
### 6、running函数
#### 首先将输入的值用\n切割，并循环用totalPrice函数计算，最后通过一个全局变量，计算出总的价格和花费以及利润，并用dom操作写在页面上


## 运行截图
![image](http://img.chufaba.me/8a36005069419d137554d497d2236347.png)