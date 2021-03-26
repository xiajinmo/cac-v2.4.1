# 8.1.个人设置

用户可以配置平台语言偏好、修改个人信息、调试API接口、使用旧云平台版本和查看平台版本信息。

## 相关操作

HYPERX云管理平台支持用户配置个人设置，支持的功能如下：

- 语言偏好：用户可以选择云平台显示的默认语言，支持中文或英文；
- 个人设置：支持用户修改头像、个人信息、密码，查看API信息；
- 夜间模式：支持主题的切换；
- 调试API接口：支持查看API接口文档，输入API密钥调试调用平台提供的API接口；
- 授权信息：支持查看平台的授权信息；
- 平台版本号：支持查看当前平台的版本信息。


操作入口如下：

- 云平台右上角个人头像(用户名)处


## 操作说明

### 设置语言偏好

云平台支持中文和英文，用户可以选择两种语言中的任何一种作为系统语言，本节将介绍默认语言的选择。

① 点击云平台右上角个人头像(用户名)处的菜单，选择“English”：

<img src="personal_settings.assets/image-20210208145353495.png" alt="image-20210208145353495" style="zoom:50%;" />

② 即可设置云平台默认语言为英文：

![image-20210127112802596](personal_settings.assets/image-20210127112802596.png)

③ 点击云平台右上角个人头像(用户名)处的菜单，选择“中文”：

<img src="personal_settings.assets/image-20210208145332102.png" alt="image-20210208145332102" style="zoom:50%;" />

④ 即可设置云平台默认语言为中文：

![image-20210127112846803](personal_settings.assets/image-20210127112846803.png)

### 个人设置

① 点击云平台右上角个人头像(用户名)处的菜单，选择“个人设置”菜单：

<img src="personal_settings.assets/image-20210208145257341.png" alt="image-20210208145257341" style="zoom:50%;" />

② 将会进入个人设置的页面，修改相关信息后点击“保存”按钮，即可配置用户个人信息：

![image-20201228115709783](personal_settings.assets/image-20201228115709783.png)

> [!NOTE]
>
> - 用户头像：用户可以点击头像，上传用户头像，用户头像尺寸须小于25*25像素，大小须小于1MB；
> - 个人信息：用户可以修改用户名、邮箱、显示名等信息，修改完成后点击“保存”按钮更新个人信息；
> - 用户的公司、部门和角色不支持在“个人设置”中进行修改，只支持查阅；
> - 用户输入的密码应至少包含一个大写字母、一个数字和一个特殊字符且不小于8位；
> - 若为该用户启用API功能，则该用户可以查看API密钥和Secret密钥用于调试API接口文档；
> - 如需开启用户API，查阅用户管理章节。

### 夜间模式

云平台支持主题的切换，本节将介绍主题切换的方法。

① 点击云平台右上角个人头像(用户名)处的菜单，打开“夜间模式”：

<img src="personal_settings.assets/image-20210208145203902.png" alt="image-20210208145203902" style="zoom:50%;" />

② 即可进入云平台的夜间模式：

![image-20210127113028799](personal_settings.assets/image-20210127113028799.png)

### 调试API接口

云平台支持为用户使用API文档调试API接口，本节将介绍API接口的类型及基本使用方法。

① 点击云平台右上角个人头像(用户名)处的菜单，选择“API”菜单：

<img src="personal_settings.assets/image-20210208145101567.png" alt="image-20210208145101567" style="zoom:50%;" />

② 即可进入API的调试接口界面：

<img src="personal_settings.assets/1597803986755.png" alt="1597803986755" style="zoom:50%;" />

③ 选择需要进行调试的API，点击“Expand Operations”按钮，将会弹出该API的详情列表：

<img src="personal_settings.assets/image-20201226095151765.png" alt="image-20201226095151765" style="zoom:50%;" />

④ 依据API的规范用例填写相应的调试参数后，点击“Try it out！”按钮：

<img src="personal_settings.assets/image-20201226095343654.png" alt="image-20201226095343654" style="zoom:50%;" />

⑤ 可获取调用API的返回值。并且可以根据表格下方提供的结果参考判断调用的结果：

<img src="personal_settings.assets/1597804212674.png" alt="1597804212674" style="zoom:50%;" />


API的详情链表由规范用例、调试参数和结果参考组成。

- 规范用例：显示调用该API的请求头示例；
- 调试参数：输入调用该API的参数、用户的API密钥和Secret密钥；
- 结果参考：显示返回值对应的结果参考，用户可以通过返回值判断调用API的问题和结果。

### 授权信息

云平台支持用户查看云平台的授权信息。

① 点击云平台右上角个人头像(用户名)处的菜单，选择“授权信息”菜单：

<img src="personal_settings.assets/image-20210208144814293.png" alt="image-20210208144814293" style="zoom:50%;" />

② 将会弹出“授权信息”的浮框，显示云平台到期的时间：

<img src="personal_settings.assets/image-20210208144834161.png" alt="image-20210208144834161" style="zoom:50%;" />

### 查看平台版本号

云平台支持用户查看当前平台的版本信息。

在左侧导航栏底部，即可看到云平台的版本号信息：

<img src="personal_settings.assets/image-20210208145024100.png" alt="image-20210208145024100" style="zoom: 67%;" />