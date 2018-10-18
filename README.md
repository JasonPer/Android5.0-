# Android5.0-后的新特性
## Android 5.0
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
#### Android 5.0 版本新增了[CardView](https://www.jianshu.com/p/63751afe368b)
### 3种 Notification
#### Android实现3种[Notification](https://www.jianshu.com/p/a84ddaf530ec)(状态栏通知)
### Toolbar 和 Palette
#### 应用内容的标准工具栏 [Toolbar](https://www.jianshu.com/p/d8b2ac97fae6)
#### Palette 的应用（Android 进阶之光 28-29页）
## Android 6.0
### 概述
#### 1.应用权限管理
#### 2.Android Pay
#### 3.指纹支持
#### 4.Doze 电量管理
#### 5.App Links
#### 6.Now on Tap
### 运行时权限机制
#### [运行时权限详解](https://www.jianshu.com/p/d4a9855e92d3)
## Android 7.0
### 概述
#### 1.多窗口模式
#### 2.Data Saver
#### 3.改进的 Java 8 语言支持
#### 4.自定义壁纸
#### 5.快速回复
#### 6.Daydream VR 支持
#### 7.后台省电
#### 8.快速设置
#### 9.Unicode 9 支持和全新的 emoji 表情符号
#### 10.[Google Assistant](http://www.sohu.com/a/231557851_114819)
## Android 8.0
### 概述
#### 1.画中画
     画中画（Picture in Picture），简称 PIP。画中画就是一个画面中浮动着另外一个画面，其实就是画面的层次感。画中画最早用于 Android TV，从 Android 8.0 开始，API 开放给所有 Android 设备。其实在 Android 的旧版本，也可以利用 Android 窗口设计框架，在其它应用上面绘制 UI 的功能，实现类似的功能。国内的某信的视频通话就是基于 Android 这一特点。当然，Android 推出画中画功能，会更加便捷的实现同样的功能。
     Android 的画中画是基于整个 Activity 的，并不是单纯的一个 View，因此，这里就会设计到 Activity 的生命周期的问题，所以画中画也会和 Activity 的生命周期绑定在一起，形成画中画生命周期。画中画的生命周期和 Android 7.0 推出的分屏模式的生命周期是一样的，只有当前和用户交互的 Activity 是最上层的 Activity，其它的可见的 Activity 都是 paused 状态。所以在处理画中画或者分屏模式需要注意 Activity 的生命周期。
#### 2.自适应图标 — Adaptive Icons
     Android 的屏幕适配一直以来都折磨着不少的开发者。为了帮助开发者更好的与设备 UI 集成，Android O 支持创建自适应图标，系统可以基于设备选择的蒙版将这些图标显示为不同形状。系统还将实现与图标的自动交互，并在启动器、快捷方式、设置、共享对话框以及概览屏幕中使用它们。
#### 3.固定快捷方式和小部件 — Pinning shortcuts
     Pinning shortcuts 是一个比 APP shortcuts 更小的快捷方式，放置于桌面上，用于更快速的打开某一 APP 的某单一任务。Pinning shortcuts 在桌面上可呈现不同的图标显示。
#### 4.Android O 其他特性介绍
     除了以上几个新特性以外，Android O 还未增加了其他的功能。比如增加了 Autofill Framework，方便用户在不同 APP 之间填写信息。比如开放 android.permission.ANSWER_PHONE_CALLS，以后在自己的 APP 里也可以对来电做响应。在性能优化上，Android O 还对隐式广播、后台服务和位置更新等进行了后台自动限制，以此来增加手机电池寿命。并对 Java 8 Language API 和 Runtime 进行了优化，使应用的运行速度更快，手机使用更流畅。
## Android 9.0
### 概述
#### 1.室内WIFI定位
      Android P增加了对RTT Wi-Fi协议的支持，以此作为室内定位的基础。 
在支持硬件支持的Android P设备上，开启定位并且打开WIFI扫描后就可以使用该功能进行定位。应用可以测量与附近支持RTT的Wi-Fi接入点（AP）的距离。设备必须启用位置并启用Wi-Fi扫描（在设置>位置下）。使用这个功能不会连接到WIFI，而且为了保持隐私，只有手机能确定AP到设备的距离，反之则不能。 
如果设备测量到3个或更多AP的距离，则可以使用多点定位算法来估算最适合这些测量值的设备位置。其结果通常可以精确到1至2米范围。
#### 2.“刘海”屏幕支持
#### 3.通知
      Android P还增加了许多对通知的支持。
#### 4.增强体验
      从Android 7.0开始，就优化了Android通知栏的体验。 
      在P当中，又新增了下述功能： 
      支持图像：Android P现在在手机上的消息通知中显示图像。您可以在消息上使用setData（）来显示图像。 
      会话参与者的简化支持：新的Notification.Person类用于标记参与聊天的人，包括他们的头像和URI。还有其他的一些API，现在都用Person类作为标志参数而不是CharSequence。
      将回复另存为草稿：当用户无意中关闭消息通知时，您的应用可以检索系统发送的EXTRA_REMOTE_INPUT_DRAFT来获取一些信息。 
      确定对话是否是群组对话：您可以使用setGroupConversation（）来有目的地将对话标识为群组对话或非群组对话。 
      为意图设置语义动作：setSemanticAction（）方法允许您为某个动作提供语义含义，如标记为读取，删除，回复等。 
      SmartReply
#### 5.通道设置、广播以及免打扰
      Android O引入了Notification Channels，可让您为要显示的每种类型的通知创建一个用户可自定义的频道。 Android P通过以下更改简化了通知渠道设置： 
      阻止渠道：用户现在可以在应用的通知设置中阻止整组渠道。您可以使用isBlocked（）方法来确定某个组何时被阻止，不对被阻止的组发送消息。 
此外，您的应用可以使用新的getNotificationChannelGroup（）方法查询当前渠道设置。 
      新的广播类型：Android系统现在在通知频道和频道组的阻塞状态发生变化时发送广播。拥有被阻止的频道或群组的应用可以监听这些Intent并作出相应的反应。有关这些Intent的更多信息，请参阅NotificationManager参考中更新后的常量列表。有关对广播Intent作出反应的信息，请参阅广播。 
      新的免打扰优先级类别：NotificationManager.Policy有两个新的策略常量：PRIORITY_CATEGORY_ALARMS（按优先级排列）和PRIORITY_CATEGORY_MEDIA_SYSTEM_OTHER（优先排列媒体，系统和游戏声音）
#### 6.多相机支持和相机更新
      现在，可以同时从两个或更多的物理摄像头同时获得数据流。在具有双前置或双后置摄像头的设备上，可以实现无法使用单个摄像头实现的功能，例如无缝缩放，散景 ，和立体视觉。 该API还允许您调用合理的或者融合的相机流，以便在两台或更多台相机之间自动切换。
#### 7.新的图片解码
      Android P新增了ImageDecoder类，为解码图像提供了一种更优的方法。由此可以用ImageDecoder来替换BitmapFactory和BitmapFactory.Options。更多使用方法请参见官方API。
#### 8.动画
      Android P引入了一个新的AnimatedImageDrawable类来绘制和显示GIF和WebP动画图像。 AnimatedImageDrawable与AnimatedVectorDrawable类似，因为AnimatedImageDrawable动画也是基于RenderThread工作的。 RenderThread本身在内部使用工作线程进行解码，因此解码不会干扰RenderThread。 这种实现允许您的应用拥有动画图像，而无需管理其更新或干扰应用的UI线程。
#### 9.HDR VP9视频，HEIF图像压缩和媒体API
      Android P增加了对HDR VP9 Profile 2的内置支持。
      Android P支持HEIF图像（隔壁IOS在2017年10月推的新的图片编码）编码。 
      Android P还引入了MediaPlayer2。该播放器支持使用DataSourceDesc构建的播放列表。
#### 10.JobScheduler中的数据成本敏感度
      在Android P当中，JobScheduler得到了改进，使其能够更好地为用户处理与网络相关的工作，并配合运营商分别提供网络状态信号。 
Jobs现在可以定义出其估计的数据大小，预取信号，并指定详细的网络要求 - 运营商可以将网络报告为拥塞或不用流量计费的。然后，JobScheduler根据网络状态管理工作。例如，当网络拥塞时，JobScheduler可能推迟大型网络请求。在不用流量计费的的网络上时，JobScheduler可以预读来改进用户体验。
#### 11.神经网络API 1.1
      对神经网络API新增了9个功能：Pad, BatchToSpaceND, SpaceToBatchND, Transpose, Strided Slice, Mean, Div, Sub, and Squeeze。
#### 12.改进表单自动填充
      Android 8.0（API26）引入了自动填充框架，这使得在应用中填写表单变得更加容易。 Android P引入了自动填充服务并实现了多项改进，以在填写表单时进一步增强用户体验。 有关更多详细信息，请参阅自动填充框架。 
      注：该自动填充框架笔者应是Google服务中的内容，国内用户可能会体验不到（或许有厂商自己的版本）。
#### 13.安全增强
      Android P引入了许多新的安全功能，包括统一的指纹验证对话框和敏感交易的高确信度的用户确认。 有关更多详细信息，请参阅安全更新(https://developer.android.com/preview/features/security.html)页面。
#### 14.Android 备份加密
      Android P支持使用客户端密钥对Android备份进行加密。 这项隐私措施，需要设备的PIN，图案密码或标准密码才能从用户设备备份的数据中恢复数据。 
      要了解有关在Android设备上备份数据的更多信息，请参阅数据备份概述(https://developer.android.com/guide/topics/data/backup.html)。 
