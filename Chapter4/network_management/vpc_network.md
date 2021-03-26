# 4.3.2.VPC管理

VPC是从整体网络中分割出来的逻辑隔离的网络，在该网络中用户具有完全控制权，可以定义IP地址范围、创建子网、配置路由表和网关。

VPC中可以包含多个独立的子网，各个子网共用同一个路由器，且每个子网都拥有独立的访问控制列表(ACL)。

在资源管理菜单下选择左侧“网络”的导航菜单，之后点击“专有网络(VPC)”的子菜单，即可看到VPC的管理界面：

![image-20210126115754539](vpc_network.assets/image-20210126115754539.png)

## 相关操作

HYPERX云管理平台支持用户对VPC进行管理，支持的功能如下：

### 特色操作

- 快速搜索：用户可以根据VPC网络的名称、说明、公司等字段全局搜索VPC网络；
- 自定义表头：用户可以从“列选择器”中自定义VPC管理界面列表显示的表头(如名称、说明、公司等)；
- 高级筛选：用户可以从表头右侧根据VPC的名称、说明、公司等字段筛选出符合条件的VPC；

### VPC相关操作

- 
  创建VPC：用户可以创建一个VPC网络；
- 编辑VPC：用户可以编辑选定的VPC网络；
- 重启VPC：用户可以重启选定的VPC网络；
- 删除VPC：用户可以删除选定的VPC网络；

### 子网相关操作

#### 子网基础操作

- 创建子网：在VPC中创建一个子网；
- 编辑子网：编辑VPC中子网的信息；
- 替换子网ACL：用户可以替换VPC中子网的ACL；
- 重启子网：用户可以重启VPC中的选定子网；
- 删除子网：用户可以删除VPC中选定的子网；

#### 内部LB

- 添加子网内部LB：用户可以在子网中添加内部负载均衡规则；
- 添加子网内部LB的虚拟机：用户可以编辑子网内部负载均衡的虚拟机；
- 删除子网内部LB的虚拟机：用户可以编辑子网内部负载均衡的虚拟机；
- 删除子网内部LB：用户可以删除子网中的内部负载均衡规则；

### 路由器相关操作

#### 公网IP

##### 公网IP基础操作

- 获取公网IP：获取新的公网IP;
- 释放公网IP：释放选定的公网IP;

##### 静态NAT

- 启用公网IP静态NAT：将选定虚拟机的IP地址与公网IP的地址绑定；
- 关闭公网IP静态NAT：解除虚拟机IP地址与公网IP的地址的绑定关系；

##### 端口转发

- 创建公网IP端口转发规则：为选定的公网IP创建端口转发规则；
- 删除公网IP端口转发规则：删除选定的端口转发规则；

##### 负载均衡

- 创建公网IP负载均衡规则：为选定的公网IP创建负载均衡规则；
- 编辑公网IP负载均衡算法：编辑选定负载均衡规则的算法；
- 编辑公网IP负载均衡粘性配置：编辑选定负载均衡规则的粘性配置；
- 添加虚拟机至公网IP负载均衡规则：将选定的虚拟机添加到选定负载均衡规则中；
- 将虚拟机从公网IP负载均衡规则中移除：将选定的虚拟机从选定负载均衡规则中移除；
- 删除公网IP负载均衡规则：删除选定的负载均衡规则；

##### VPN

- 启用公网IP的VPN：启用公网IP的VPN服务，将虚拟机路由器作为VPN的服务网关；
- 创建公网IP的VPN用户：添加可以使用VPN的用户；
- 删除公网IP的VPN用户：删除选定的VPN用户；
- 禁用公网IP的VPN：禁用公网IP的VPN服务，用户不得通过VPN登录；

#### 点到点VPN

- 添加点到点VPN网关：将选定路由器的公网IP配置为点到点的VPN网关；
- 查看点到点VPN网关详情：查看点到点VPN网关的详情信息，包括ID、组织等相关信息；
- 删除点到点VPN网关：删除选定的点到点VPN网关；
- 添加点到点VPN连接：添加一个点到点VPN连接；
- 重启点到点VPN连接：重新启动选定的点到点VPN连接；
- 删除点到点VPN连接：删除选定的点到点VPN连接；

#### 网络ACL

- 添加ACL：在路由器中添加一个ACL；
- 添加ACL规则：在ACL中添加一条ACL规则；
- 编辑ACL规则：编辑选定的ACL规则；
- 删除ACL规则：删除选定的ACL规则；
- 删除ACL：删除选定的ACL。


操作入口如下：

-  资源管理→网络→VPC

## 操作说明

### VPC相关操作

#### 创建VPC

① 在VPC管理界面中，点击“创建VPC”按钮：

![image-20201223115441911](vpc_network.assets/image-20201223115441911.png)

② 在弹出的操作提示框中填写VPC的名称、组织、IP网段等信息后，点击“确定”按钮添加VPC：

<img src="vpc_network.assets/image-20210225122140425.png" alt="image-20210225122140425" style="zoom:50%;" />

#### 编辑VPC

① 在VPC管理界面中，点击操作列的“编辑VPC”按钮：

![image-20210225115905932](vpc_network.assets/image-20210225115905932.png)

② 将会进入编辑VPC的页面，修改VPC的名称或备注后，点击“确定”按钮编辑VPC的相关信息：

![image-20210225120032474](vpc_network.assets/image-20210225120032474.png)

#### 重启VPC

① 在VPC管理界面中，选择需要重启的VPC，点击操作列的“重启VPC”按钮：

![image-20210225124934772](vpc_network.assets/image-20210225124934772.png)

② 将会弹出“重启VPC”的操作提示框，点击“确定”按钮后，重启选定的VPC网络：

<img src="vpc_network.assets/image-20201223121848868.png" alt="image-20201223121848868" style="zoom:50%;" />

> [!WARNING]
>
> - 若勾选“重置虚拟路由”复选框，将会删除现有虚拟路由并且重建新的虚拟路由；
>
> - 若勾选“冗余”按钮，将非冗余VPC改为冗余VPC，会新建一个虚拟路由。
>

#### 删除VPC

① 在VPC管理界面中，点击操作列的“删除VPC”按钮：

![image-20210225125720396](vpc_network.assets/image-20210225125720396.png)

② 将会弹出“删除”的操作提示框，点击“确定”按钮后，删除选定的VPC网络：

<img src="vpc_network.assets/image-20210121190955403.png" alt="image-20210121190955403" style="zoom:50%;" />

> [!WARNING]
>
> - 删除VPC网络前，需要删除VPC中全部的子网。
>

### 子网相关操作

#### 子网基础操作

##### 创建子网

① 在VPC管理界面中，点击需要创建子网的VPC的名称，进入VPC的详情页：

![image-20210225125058883](vpc_network.assets/image-20210225125058883.png)

② 在“子网”选项卡中，点击“创建子网”按钮：

![image-20210121191114124](vpc_network.assets/image-20210121191114124.png)

③ 在弹出的“创建子网”操作提示框中填写名称、网络网段、ACL等信息后，点击“确定”按钮创建VPC的子网：

<img src="vpc_network.assets/image-20210225120558861.png" alt="image-20210225120558861" style="zoom:50%;" />

##### 编辑子网

① 在VPC管理界面中，点击需要编辑子网的VPC的名称，进入VPC的详情页：

![image-20210225125114391](vpc_network.assets/image-20210225125114391.png)

② 在“子网”选项卡中，选择需要编辑的子网， 点击操作列的“编辑子网”按钮：

![image-20210226094236462](vpc_network.assets/image-20210226094236462.png)

③ 进入编辑子网的页面，修改子网的名称、说明等信息后，点击“确定”按钮编辑VPC的子网：

<img src="vpc_network.assets/image-20210226094658344.png" alt="image-20210226094658344" style="zoom:50%;" />

##### 替换子网ACL

① 在VPC管理界面中，点击需要替换子网ACL的VPC的名称，进入VPC的详情页：

![image-20210225125124632](vpc_network.assets/image-20210225125124632.png)

② 在“子网”选项卡中，选择需要替换ACL的子网， 点击操作列的“替换ACL”按钮：

![image-20210226094910842](vpc_network.assets/image-20210226094910842.png)

③ 将会弹出“替换ACL”的操作提示框，修改ACL后，点击“确定”按钮：

<img src="vpc_network.assets/image-20210126120958961.png" alt="image-20210126120958961" style="zoom:50%;" />

##### 重启子网

① 在VPC管理界面中，点击需要编辑子网的VPC的名称，进入VPC的详情页：

![image-20210225125132885](vpc_network.assets/image-20210225125132885.png)

② 在“子网”选项卡中，选择需要重启的子网，点击操作列的“重启子网”按钮：

![image-20210226100146308](vpc_network.assets/image-20210226100146308.png)

③ 将会弹出“重启网络”的操作提示框，点击“确定”按钮后，重启选定的网络：

<img src="vpc_network.assets/image-20210127183156362.png" alt="image-20210127183156362" style="zoom:50%;" />

##### 删除子网

① 在VPC管理界面中，点击需要删除子网的VPC的名称，进入VPC的详情页：

![image-20210225125140961](vpc_network.assets/image-20210225125140961.png)

② 在“子网”选项卡中，选择需要删除的子网，点击操作列的“删除子网”按钮：

![image-20210226100321084](vpc_network.assets/image-20210226100321084.png)

③ 将会弹出“删除网络”的操作提示框，点击“确定”按钮后，删除选定的子网：

<img src="vpc_network.assets/image-20210127183116117.png" alt="image-20210127183116117" style="zoom:50%;" />

#### 内部LB

##### 添加VPC子网内部LB

① 在VPC管理界面中，点击需要添加子网内部LB的VPC的名称，进入VPC的详情页：

![image-20210225125146181](vpc_network.assets/image-20210225125146181.png)

② 在“子网”选项卡中，选择需要添加内部LB的子网，点击子网“内部LB”的数字：

![image-20210226100455593](vpc_network.assets/image-20210226100455593.png)

③ 进入子网内部LB的界面，点击“添加内部LB”按钮：

![image-20210127121519353](vpc_network.assets/image-20210127121519353.png)

④ 弹出“添加内部LB”的操作提示框，填写相关信息后，点击“创建”按钮添加子网内部的LB：

<img src="vpc_network.assets/image-20201225155416589.png" alt="image-20201225155416589" style="zoom:50%;" />

##### 添加子网内部LB虚拟机

① 在VPC管理界面中，点击需要添加子网内部LB虚拟机的VPC的名称，进入VPC的详情页：

![image-20210225125156648](vpc_network.assets/image-20210225125156648.png)

② 在“子网”选项卡中，选择需要添加子网内部LB虚拟机的子网，点击子网“内部LB”的数字：

![image-20210226100939121](vpc_network.assets/image-20210226100939121.png)

③ 进入子网内部LB的界面，选择需要添加虚拟机的内部LB，点击操作列的“添加”按钮：

![image-20210127121540269](vpc_network.assets/image-20210127121540269.png)

④ 将会弹出“配置虚拟机”的操作提示框，选择虚拟机和IP后，点击“添加”按钮添加子网内部LB的虚拟机：

<img src="vpc_network.assets/image-20210127121600059.png" alt="image-20210127121600059" style="zoom:50%;" />

##### 删除子网内部LB虚拟机

① 在VPC管理界面中，点击需要删除子网内部LB虚拟机的VPC的名称，进入VPC的详情页：

![image-20210225125204338](vpc_network.assets/image-20210225125204338.png)

② 在“子网”选项卡中，选择需要编辑子网内部LB虚拟机的子网，点击子网“内部LB”的数字：

![image-20210226100949579](vpc_network.assets/image-20210226100949579.png)

③ 点击“更多”小箭头，将会显示子网内部LB的虚拟机：

![image-20210127121815102](vpc_network.assets/image-20210127121815102.png)

④ 选择需要删除的子网内部LB的虚拟机，点击操作列的“删除”按钮：

![image-20210127121648734](vpc_network.assets/image-20210127121648734.png)

⑤ 将会弹出“确认删除”的操作提示框，点击“确定”按钮删除选定的子网内部LB的虚拟机：

<img src="vpc_network.assets/image-20210127121708599.png" alt="image-20210127121708599" style="zoom:50%;" />

##### 删除子网内部LB

① 在VPC管理界面中，点击需要删除子网内部LB的VPC的名称，进入VPC的详情页：

![image-20210225125209336](vpc_network.assets/image-20210225125209336.png)

② 在“子网”选项卡中，选择需要删除内部LB的子网，点击子网“内部LB”的数字：

![image-20210226101008268](vpc_network.assets/image-20210226101008268.png)

③ 进入子网内部LB的界面，选择需要删除的内部LB，点击操作列的“删除”按钮：

![image-20210127121858860](vpc_network.assets/image-20210127121858860.png)

④ 将会弹出“删除内部LB”的操作提示框，点击“确定”按钮删除选定的子网内部LB：

<img src="vpc_network.assets/image-20210127121919592.png" alt="image-20210127121919592" style="zoom:50%;" />

### 路由器相关操作

#### 公网IP

##### 公网IP基础操作

###### 获取公网IP

① 在VPC管理界面中，点击需要获取公网IP的VPC的名称，进入VPC的详情页：

![image-20210225125216870](vpc_network.assets/image-20210225125216870.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击“获取新的公网IP”按钮：

![image-20210122094803339](vpc_network.assets/image-20210122094803339.png)

③ 将会弹出“获取新的公网IP”操作提示框，点击“确定”按钮获取新的公网IP:

<img src="vpc_network.assets/image-20210122094829867.png" alt="image-20210122094829867" style="zoom:50%;" />

###### 释放公网IP

① 在VPC管理界面中，点击需要释放公网IP的VPC的名称，进入VPC的详情页：

![image-20210225125222451](vpc_network.assets/image-20210225125222451.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，选择需要释放的公网IP，点击操作列的“释放IP”按钮：

![image-20210126121433927](vpc_network.assets/image-20210126121433927.png)

③ 将会弹出“释放”的操作提示框，点击“确定”按钮释放选定的公网IP：

<img src="vpc_network.assets/image-20210127183239995.png" alt="image-20210127183239995" style="zoom:50%;" />

##### 静态NAT

###### 启用公网IP静态NAT

① 在VPC管理界面中，点击需要启用公网IP静态NAT的VPC的名称，进入VPC的详情页：

![image-20210225125226906](vpc_network.assets/image-20210225125226906.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击需要启用静态NAT的公网IP名称：

![image-20210126121558952](vpc_network.assets/image-20210126121558952.png)

③ 进入公网IP详情页，点击“启用静态NAT”按钮：

![image-20210122174513228](vpc_network.assets/image-20210122174513228.png)

④ 将会弹出“启用静态NAT”操作提示框，填写相关信息后点击“确定”按钮即可启用选定公网IP的静态NAT：

<img src="vpc_network.assets/image-20210122174435729.png" alt="image-20210122174435729" style="zoom:50%;" />

> [!WARNING]
>
> - 公网IP启用静态NAT后，不支持配置端口转发和负载均衡规则。

###### 关闭公网IP静态NAT

① 在VPC管理界面中，点击需要关闭公网IP静态NAT的VPC的名称，进入VPC的详情页：

![image-20210225125232569](vpc_network.assets/image-20210225125232569.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击需要关闭静态NAT的公网IP名称：

![image-20210126121607899](vpc_network.assets/image-20210126121607899.png)

③ 进入公网IP详情页，点击“关闭静态NAT”按钮：

![image-20210122175147446](vpc_network.assets/image-20210122175147446.png)

④ 将会弹出“关闭静态NAT”的操作提示框，点击“确定”按钮可关闭选定公网IP的静态NAT：

<img src="vpc_network.assets/image-20210122175206604.png" alt="image-20210122175206604" style="zoom:50%;" />

##### 端口转发

###### 创建公网IP端口转发规则

① 在VPC管理界面中，点击需要创建公网IP端口转发规则的VPC的名称，进入VPC的详情页：

![image-20210225125240048](vpc_network.assets/image-20210225125240048.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击创建公网IP端口转发规则的公网IP名称：

![image-20210126121612700](vpc_network.assets/image-20210126121612700.png)

③ 选择“端口转发”选项卡，点击“创建转发规则”按钮：

![image-20210122175348441](vpc_network.assets/image-20210122175348441.png)

④ 将会弹出“创建转发规则”的操作提示框，填写相关信息后点击“确定”按钮即可创建公网IP的端口转发规则：

<img src="vpc_network.assets/image-20210122175430987.png" alt="image-20210122175430987" style="zoom:50%;" />

> [!NOTE]
>
> - 公网IP配置端口转发规则后，不支持配置负载均衡规则和启用静态NAT；
> - 公网IP为某一个子网的虚拟机配置端口转发规则后，该公网IP则属于该子网专用，不再允许为VPC的其他子网配置端口转发规则；
> - 如果VPC的私有开始端口与私有结束端口不相同，则公共开始、结束端口需与私有开始、结束端口相同。

###### 删除公网IP端口转发规则

① 在VPC管理界面中，点击需要删除公网IP端口转发规则的VPC的名称，进入VPC的详情页：

![image-20210225125246869](vpc_network.assets/image-20210225125246869.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击删除公网IP端口转发规则的公网IP名称：

![image-20210126121633733](vpc_network.assets/image-20210126121633733.png)

③ 选择“端口转发”选项卡，选择需要删除的端口转发规则，点击操作列的‘’删除”按钮：

![image-20210122175815896](vpc_network.assets/image-20210122175815896.png)

④ 将会弹出“删除”的操作提示框，点击“确定”按钮即可删除选定的公网IP的端口转发规则：

<img src="vpc_network.assets/image-20210126121740795.png" alt="image-20210126121740795" style="zoom:50%;" />

##### 负载均衡

###### 创建公网IP负载均衡规则

① 在VPC管理界面中，点击需要创建公网IP负载均衡规则的VPC的名称，进入VPC的详情页：

![image-20210225125250160](vpc_network.assets/image-20210225125250160.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击创建公网IP负载均衡规则的公网IP名称：

![image-20210126121623562](vpc_network.assets/image-20210126121623562.png)

③ 选择“负载均衡”选项卡，点击操作列的‘’创建规则”按钮：

![image-20210122180316471](vpc_network.assets/image-20210122180316471.png)

④ 将会弹出“创建规则”的操作提示框，填写相关信息后点击“下一步”按钮：

<img src="vpc_network.assets/image-20210122180427153.png" alt="image-20210122180427153" style="zoom:50%;" />

⑤ 选择负载均衡的虚拟机后，点击“确定”按钮即可创建公网IP的负载均衡规则：

<img src="vpc_network.assets/image-20210122180726896.png" alt="image-20210122180726896" style="zoom:50%;" />

> [!WARNING]
>
> - 公网IP配置负载均衡规则后，不支持配置端口转发规则和启用静态NAT；
> - 公网IP为某一个子网的虚拟机配置负载均衡规则后，该公网IP则属于该子网专用，不再允许为VPC的其他子网配置负载均衡规则。

######  编辑公网IP负载均衡算法

① 在VPC管理界面中，点击需要编辑公网IP负载均衡规则的VPC的名称，进入VPC的详情页：

![image-20210225125257909](vpc_network.assets/image-20210225125257909.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击编辑公网IP负载均衡规则的公网IP名称：

![image-20210126121633733](vpc_network.assets/image-20210126121633733.png)

③ 在“负载均衡”选项卡中，选择需要编辑算法的负载均衡规则，点击操作列的“编辑算法”按钮：

![image-20210126122554278](vpc_network.assets/image-20210126122554278.png)

④ 将会弹出“编辑规则”的操作提示框，编辑算法后点击“确定”按钮即可：

<img src="vpc_network.assets/image-20210126122136742.png" alt="image-20210126122136742" style="zoom:50%;" />

######  编辑公网IP负载均衡粘性配置 

① 在VPC管理界面中，点击需要编辑公网IP负载均衡规则的VPC的名称，进入VPC的详情页：

![image-20210225125303396](vpc_network.assets/image-20210225125303396.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击编辑公网IP负载均衡规则的公网IP名称：

![image-20210126121633733](vpc_network.assets/image-20210126121633733.png)

③ 在“负载均衡”选项卡中，选择需要编辑粘性规则的负载均衡规则，点击操作列的“编辑粘性规则”按钮：

![image-20210126122618040](vpc_network.assets/image-20210126122618040.png)

④ 将会弹出“编辑粘性规则”的操作提示框，编辑粘性规则后点击“确定”按钮即可：

<img src="vpc_network.assets/image-20210127180905234.png" alt="image-20210127180905234" style="zoom:50%;" />

######  添加虚拟机至公网IP负载均衡规则 

① 在VPC管理界面中，点击需要编辑公网IP负载均衡规则虚拟机的VPC的名称，进入VPC的详情页：

![image-20210225125309394](vpc_network.assets/image-20210225125309394.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击编辑公网IP负载均衡规则虚拟机的公网IP名称：

![image-20210126121633733](vpc_network.assets/image-20210126121633733.png)

③ 在“负载均衡”选项卡中，选择需要加载虚拟机的负载均衡规则，点击操作列的“添加虚机”按钮：

![image-20210126122644739](vpc_network.assets/image-20210126122644739.png)

④将会弹出“配置虚拟机”的操作提示框，选择虚拟机后点击“确定”按钮即可：

<img src="vpc_network.assets/image-20210126122944961.png" alt="image-20210126122944961" style="zoom:50%;" />

######  将虚拟机从公网IP负载均衡规则中移除 

① 在VPC管理界面中，点击需要编辑公网IP负载均衡规则虚拟机的VPC的名称，进入VPC的详情页：

![image-20210225125314123](vpc_network.assets/image-20210225125314123.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击编辑公网IP负载均衡规则虚拟机的公网IP名称：

![image-20210126121633733](vpc_network.assets/image-20210126121633733.png)

③ 在“负载均衡”选项卡中， 选择需要移除虚拟机的负载均衡规则，点击“更多”拓展标识，显示该负载均衡规则关联的虚拟机：

![image-20210126123245580](vpc_network.assets/image-20210126123245580.png)

④ 选择移除虚拟机的负载均衡规则，点击操作列的“删除”按钮： 

![image-20210126123121537](vpc_network.assets/image-20210126123121537.png)

⑤ 将会弹出“删除”的操作提示框，点击“确定”按钮，即可移除负载均衡规则中选定的虚拟机 ：

<img src="vpc_network.assets/image-20210126123144558.png" alt="image-20210126123144558" style="zoom:50%;" />

###### 删除公网IP负载均衡规则

① 在VPC管理界面中，点击需要删除公网IP负载均衡规则的VPC的名称，进入VPC的详情页：

![image-20210225125320529](vpc_network.assets/image-20210225125320529.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，点击删除负载均衡规则的公网IP名称：

![image-20210126121633733](vpc_network.assets/image-20210126121633733.png)

③ 在“负载均衡”选项卡中，选择需要删除的负载均衡规则，点击操作列的“删除”按钮：

![image-20210126122751826](vpc_network.assets/image-20210126122751826.png)

④ 将会弹出“删除”的操作提示框，点击“确定”按钮即可删除选定的负载均衡规则：

<img src="vpc_network.assets/image-20210126122830863.png" alt="image-20210126122830863" style="zoom:50%;" />

##### VPN

###### 启用公网IP的VPN

① 在VPC管理界面中，点击需要启用公网IP的VPN的VPC的名称，进入VPC的详情页：

![image-20210225125326339](vpc_network.assets/image-20210225125326339.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，选择需要启用VPN的公网IP，点击操作列的“启用VPN”按钮：

![](vpc_network.assets/image-20210126123520053.png)

③ 将会弹出“启用远程访问VPN”的操作提示框，点击“确定”按钮即可启用远程访问VPN：

<img src="vpc_network.assets/image-20210127121241658.png" alt="image-20210127121241658" style="zoom:50%;" />

###### 显示VPN的IPSec预共享秘钥

① 在VPC管理界面中，点击需要显示VPN的IPSec预共享秘钥的VPC的名称，进入VPC的详情页：

![image-20210225125330875](vpc_network.assets/image-20210225125330875.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，选择需要显示VPN的IPSec预共享秘钥的公网IP名称：

![image-20210126123715686](vpc_network.assets/image-20210126123715686.png)

③ 选择“VPN”选项卡，点击“显示密钥”按钮：
![image-20210126123807121](vpc_network.assets/image-20210126123807121.png)

④ 即可看到IPSec预共享密钥：

<img src="vpc_network.assets/image-20210126123831663.png" alt="image-20210126123831663" style="zoom:50%;" />

###### 创建VPN用户

① 在VPC管理界面中，点击需要创建VPN用户的VPC的名称，进入VPC的详情页：

![image-20210225125335625](vpc_network.assets/image-20210225125335625.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，选择需要创建VPN用户的公网IP名称：

![image-20210126123722007](vpc_network.assets/image-20210126123722007.png)

③ 选择“VPN”选项卡，点击“创建VPN用户”按钮：

![image-20210127121044858](vpc_network.assets/image-20210127121044858.png)

④ 将会弹出“创建VPN用户”的操作提示框，填写用户名和密码后，点击“确定”按钮，即可为选定的VPN添加用户：

<img src="vpc_network.assets/image-20210127121003610.png" alt="image-20210127121003610" style="zoom:50%;" />

###### 删除VPN用户

① 在VPC管理界面中，点击需要删除VPN用户的VPC的名称，进入VPC的详情页：

![image-20210225125341059](vpc_network.assets/image-20210225125341059.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，选择需要删除VPN用户的公网IP名称：

![image-20210126123725693](vpc_network.assets/image-20210126123725693.png)

③ 选择“VPN”选项卡，选择需要删除的用户，点击操作列的“删除”按钮：

![image-20210127121121115](vpc_network.assets/image-20210127121121115.png)

④ 将会弹出“删除用户的操作提示框，点击“确定”按钮即可删除选定的VPN用户：

<img src="vpc_network.assets/image-20210126124806058.png" alt="image-20210126124806058" style="zoom:50%;" />

###### 禁用公网IP的VPN

① 在VPC管理界面中，点击需要禁用公网IP的VPN的VPC的名称，进入VPC的详情页：

![image-20210225125345710](vpc_network.assets/image-20210225125345710.png)

② 在“路由器”选项卡中，选择“公网IP地址”子选项卡，选择需要禁用VPN的公网IP，点击操作列的“禁用VPN”按钮：

![image-20210127121201640](vpc_network.assets/image-20210127121201640.png)

③ 将会弹出“禁用VPN”的操作提示框，点击“确定”按钮即可禁用远程访问VPN：

<img src="vpc_network.assets/image-20210127120805355.png" alt="image-20210127120805355" style="zoom:50%;" />



#### 点到点VPN

##### 添加点到点VPN网关

① 在VPC管理界面中，点击需要添加点到点VPN网关的VPC的名称，进入VPC的详情页：

![image-20210225125350435](vpc_network.assets/image-20210225125350435.png)

② 在“路由器”选项卡中，选择“点到点VPN”子选项卡，点击“添加点到点VPN网关”按钮：

![image-20201225140552291](vpc_network.assets/image-20201225140552291.png)

③ 将会弹出“创建VPN网关”的操作提示框，点击“确定”按钮即可添加点到点VPN网关：

<img src="vpc_network.assets/image-20201225140617693.png" alt="image-20201225140617693" style="zoom:50%;" />

##### 查看点到点VPN网关详情

① 在VPC管理界面中，点击需要查看点到点VPN网关的VPC的名称，进入VPC的详情页：

![image-20210225125355414](vpc_network.assets/image-20210225125355414.png)

② 在“路由器”选项卡中，选择“点到点VPN”子选项卡，选择需要查看的点到点VPN，点击操作列的“详情”按钮：

![image-20210121193105863](vpc_network.assets/image-20210121193105863.png)

③ 即可查看点到点VPN网关的详情信息：

<img src="vpc_network.assets/image-20210121193119792.png" alt="image-20210121193119792" style="zoom:50%;" />

##### 删除点到点VPN网关

① 在VPC管理界面中，点击需要删除点到点VPN网关的VPC的名称，进入VPC的详情页：

![image-20210225125400071](vpc_network.assets/image-20210225125400071.png)

② 在“路由器”选项卡中，选择“点到点VPN”子选项卡，选择需要删除的点到点VPN，点击操作列的“删除”按钮：

![image-20210121193209211](vpc_network.assets/image-20210121193209211.png)

③ 将会弹出“删除”的操作提示框，点击“确定”按钮即可删除选定的点到点VPN网关：

<img src="vpc_network.assets/image-20210121193230787.png" alt="image-20210121193230787" style="zoom:50%;" />

> [!WARNING]
>
> - 当且仅当VPN网关下有VPN连接时，VPN网关不支持删除。

##### 添加点到点VPN连接

① 在VPC管理界面中，点击需要添加点到点VPN连接的VPC的名称，进入VPC的详情页：

![image-20210225125404257](vpc_network.assets/image-20210225125404257.png)

② 在“路由器”选项卡中，选择“点到点VPN”下的“VPN连接”子选项卡，点击“添加VPN连接”按钮：

![image-20210121193358806](vpc_network.assets/image-20210121193358806.png)

③ 将会弹出“创建VPN连接”的操作提示框，选择VPN网关后，点击“确定”按钮即可添加点到点VPN连接：

<img src="vpc_network.assets/image-20210121193557112.png" alt="image-20210121193557112" style="zoom:50%;" />

##### 查看点到点VPN连接

① 在VPC管理界面中，点击需要添加点到点VPN连接的VPC的名称，进入VPC的详情页：

![image-20210225125409844](vpc_network.assets/image-20210225125409844.png)

② 在“路由器”选项卡中，选择“点到点VPN”下的“VPN连接”子选项卡，选择需要查看的点到点VPN连接，点击操作列的“详情”按钮：

![image-20210121193745574](vpc_network.assets/image-20210121193745574.png)

③ 即可查看点到点VPN连接的详情信息：

<img src="vpc_network.assets/image-20210121193801376.png" alt="image-20210121193801376" style="zoom:50%;" />

##### 重启点到点VPN连接

① 在VPC管理界面中，点击需要重启点到点VPN连接的VPC的名称，进入VPC的详情页：

![image-20210225125414657](vpc_network.assets/image-20210225125414657.png)

② 在“路由器”选项卡中，选择“点到点VPN”下的“VPN连接”子选项卡，选择需要重启的点到点VPN连接，点击操作列的“重启”按钮：

![image-20210121193836665](vpc_network.assets/image-20210121193836665.png)

③ 将会弹出“重启VPN连接”的操作提示框，点击“确定”按钮即可重启选定的VPN连接：

<img src="vpc_network.assets/image-20210126125107837.png" alt="image-20210126125107837" style="zoom:50%;" />

##### 删除点到点VPN连接

① 在VPC管理界面中，点击需要删除点到点VPN连接的VPC的名称，进入VPC的详情页：

![image-20210225125418631](vpc_network.assets/image-20210225125418631.png)

② 在“路由器”选项卡中，选择“点到点VPN”下的“VPN连接”子选项卡，选择需要删除的点到点VPN连接，点击操作列的“删除”按钮：

![image-20210121194058512](vpc_network.assets/image-20210121194058512.png)

③ 将会弹出“删除”的操作提示框，点击“确定”按钮即可删除选定的VPN连接：

<img src="vpc_network.assets/image-20210121194230158.png" alt="image-20210121194230158" style="zoom:50%;" />

####  网络ACL

##### 添加ACL

① 在VPC管理界面中，点击需要添加ACL的VPC的名称，进入VPC的详情页：

![image-20210225125422995](vpc_network.assets/image-20210225125422995.png)

② 在“路由器”选项卡中，选择“访问控制列表(ACL)”子选项卡，点击“添加ACL”按钮：

![image-20210121194340702](vpc_network.assets/image-20210121194340702.png)

③ 将会弹出“添加ACL”的操作提示框，填写相关信息后点击“确定”按钮即可成功添加ACL：

<img src="vpc_network.assets/image-20210121191434018.png" alt="image-20210121191434018" style="zoom:50%;" />

##### 添加ACL规则

① 在VPC管理界面中，点击需要添加ACL规则VPC的名称，进入VPC的详情页：

![image-20210225125427996](vpc_network.assets/image-20210225125427996.png)

② 在“路由器”选项卡中，选择“访问控制列表(ACL)”子选项卡，选择需要添加规则的ACL，点击操作列的“配置ACL”按钮：

![image-20210121191619981](vpc_network.assets/image-20210121191619981.png)

③ 将会进入配置ACL的界面，点击“增加规则”按钮：

![image-20210121191757756](vpc_network.assets/image-20210121191757756.png)

④ 将会弹出“创建网络ACL规则”的操作提示框，填写相关信息后点击“确定”按钮即可添加ACL规则：

<img src="vpc_network.assets/image-20210121191851625.png" alt="image-20210121191851625" style="zoom:50%;" />

> [!NOTE]
>
> - 仅自定义的ACL支持添加ACL规则，默认的default_deny和default_allow列表不支持添加ACL规则；
> - 为保证VPC内虚拟机能正常显示监控信息，新建的ACL会自动创建监控CIDR、端口的ACL规则。

##### 编辑ACL规则

① 在VPC管理界面中，点击需要编辑ACL规则VPC的名称，进入VPC的详情页：

![image-20210225125434801](vpc_network.assets/image-20210225125434801.png)

② 在“路由器”选项卡中，选择“访问控制列表(ACL)”子选项卡，选择需要编辑规则的ACL，点击操作列的“配置ACL”按钮：

![image-20210226105957363](vpc_network.assets/image-20210226105957363.png)

③ 将会进入配置ACL的界面，选择需要编辑的ACL规则，点击操作列的“编辑ACL规则”按钮：

![image-20210121192039176](vpc_network.assets/image-20210121192039176.png)

④ 将会弹出“编辑网络ACL规则”的操作提示框，编辑相关信息后点击“确定”按钮即可成功编辑ACL规则：

<img src="vpc_network.assets/image-20210121192118261.png" alt="image-20210121192118261" style="zoom:50%;" />

##### 删除ACL规则   

① 在VPC管理界面中，点击需要删除ACL规则VPC的名称，进入VPC的详情页：

![image-20210225125439818](vpc_network.assets/image-20210225125439818.png)

② 在“路由器”选项卡中，选择“访问控制列表(ACL)”子选项卡，选择需要删除规则的ACL，点击操作列的“配置ACL”按钮：

![image-20210121191619981](vpc_network.assets/image-20210121191619981.png)

③ 将会进入配置ACL的界面，选择需要删除的ACL规则，点击操作列的“删除ACL规则”按钮：

![image-20210121192158412](vpc_network.assets/image-20210121192158412.png)

④ 将会弹出“删除”的操作提示框，点击“确定”按钮即可删除选定的ACL规则：

<img src="vpc_network.assets/image-20210121192213457.png" alt="image-20210121192213457" style="zoom:50%;" />

##### 删除ACL

① 在VPC管理界面中，点击需要删除ACLVPC的名称，进入VPC的详情页：

![image-20210225125445536](vpc_network.assets/image-20210225125445536.png)

② 在“路由器”选项卡中，选择“访问控制列表(ACL)”子选项卡，选择需要删除的ACL，点击操作列的“删除ACL”按钮：

![image-20210226105957363](vpc_network.assets/image-20210226105957363.png)

③ 将会弹出“确认删除”的操作提示框，点击“确定”按钮即可删除选定的ACL：

<img src="vpc_network.assets/image-20210122173144771.png" alt="image-20210122173144771" style="zoom:50%;" />