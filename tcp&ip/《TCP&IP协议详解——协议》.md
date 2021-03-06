> 有效的沟通取决于共同的语言。

### 基本概念

TPC/IP是一个实现Internet体系结构的协议族。

##### 命运共享原则 & 端到端论点

- 影响TCP/IP协议族设计的一个重要原则

##### 差错控制和流量控制

- 简单来说，对网络中存在数据损坏或丢失情况的处理称为`差错控制`。出现`差错控制`的原因（硬件问题、传输过程中数据被修改等）

- TCP在端主机中实现速率控制。

###　网络协议的设计和实现　＝＝＝> 分层

- OSI (开放系统互联标准)

通过分层，将各自的实现分开

### OSI 七层网络模型 & TCP/IP五层网络模型

![705728-20160424234824085-667046040.png](https://i.loli.net/2019/07/10/5d25ff73f302c44332.png)

### 基本名词&术语

- PDU （协议数据单元）

- ICMP （Internet控制消息协议）

- IGMP （Internet组管理协议）

- ARP （地址解析协议，IPv4专用协议，完成IP地址和链路层地址的转换）

IP发送给链路层协议的PDU称为IP数据报（大小为64K，IPv6扩大为4GB）

每个IP分组都是一个数据报

每个数据抱都包含发送方和接收方的IP地址

将大分组放入链路层PDU时的缩小处理称为`分片`

大数据会被放入多个称为`分片`的小数据报中，到达指定的主机后进行`重组`

将数据报发送到下一跳的过程称为`转发`

#### 转发类型

|名称|转发对象|
|:---:|:---|
|单播|一台主机|
|广播|一个指定网络中的所有主机|
|组播|一个组播组中的一组主机|

### 端口号 （0 ～ 65535）

|划分|范围|
|:---:|:---:|
|熟知端口号|（0 ~ 1023）|
|注册端口号|（1024 ～ 49151）|
|私有端口号|（49152 ～ 65535）|


> 你无法逃避生活来寻求平静。
