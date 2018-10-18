# Android5.0-后的新特性
## Android5.0
### 概述
#### 1.全新的 Material Design 设计风格
#### 2.支持多种设备
#### 3.全新的通知中心设计
#### 4.支持64位 ART 虚拟机
#### 5.Overview
#### 6.设备识别解锁
#### 7.Ok Google 语音指令
#### 8.Face unlock 面部解锁
### RecyclerView
#### 基本使用
##### 引用
      在的build.gradle中文件引入该类。
##### 布局
      活动布局文件activity_rv.xml 
      Item的布局文件item_1.xml 
##### 创建适配器
      创建一个继承RecyclerView.Adapter<VH>的Adapter类
      在适配器中创建一个继承RecyclerView.ViewHolder的静态内部类，记为VH.ViewHolder的实现和ListView的ViewHolder实现几乎一样
      在Adapter中实现3个方法：
      onCreateViewHolder（）
      onBindViewHolder（）
      getItemCount（）
##### 设置RecyclerView
      为RecyclerView进行相应设置
      布局管理
      适配器设置
      设置分割线（.addItemDecoration()方法）
      自定义点击事件
      条目动画等等
### CardView
#### Android 5.0 版本新增了CardView
    [CardView详解](https://www.jianshu.com/p/63751afe368b)
