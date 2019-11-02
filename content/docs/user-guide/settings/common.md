+++
title = "通用"
description = ""
weight = 1
+++


## 1. 概述

通用设置主要是对所属项目的基本信息、应用配置和仓库精心修改和设置。

> 通用设置必须拥有项目xxx角色权限。

![image](/docs/user-guide/settings/image/project-setting-01.png)

## 2. 基本信息

基本信息显示项目的基本信息，字段描述如下：

- 项目名称：项目的名称。
- 项目编码：项目编码具有唯一性，是项目的标识。
- 项目类型：项目的类型，标识此项目的用途。
- 状态：状态有启用和停用两种形态。当启用状态为启用时，项目正常运行，可进入该项目中进行其他操作；当启用状态为停用时，无法进入该项目。创建成功一个项目后，该项目的启用状态默认为启用。
- 项目类别：项目的类别，标识此项目是敏捷项目或是普通项目群。项目群可维护子项目。

### 2.1 修改基本信息（字段不确定需修改）

点击导航栏上方的`修改`按钮，会跳出基本信息修改页面。

![image](/docs/user-guide/settings/image/project-setting-02.png)

不可修改字段：

项目编码：项目编码具有唯一性，是项目的标识。
项目类别：默认为敏捷项目。有敏捷项目、普通项目群两种值。普通项目群可维护子项目。

可修改字段：
- 项目名称：可以对项目的名称进行修改。
- 项目类型：可以修改此项目的类型。
- 项目图标：可以修改项目的头像，更好的标识您的项目。

## 3. 应用配置

点击`应用配置`进入详情页，点击导航栏上方的`修改`按钮，会跳出修改页面，~~在此可对应用名称、来源、类型进行修改。~~

【缺图】

## 4. 仓库
点击`仓库`进入详情页，再点击导航栏上方的`修改`按钮，会从右侧弹出仓库的修改页面。

![image](/docs/user-guide/settings/image/project-setting-03.png)

1. 修改默认Docker仓库为自定义Docker仓库。
    * 将默认Docker仓库切换为自定义Docker仓库。
    * 输入仓库地址。
    * 输入登录名与密码；此处需要输入有推拉代码权限的登录名和密码。
    * 输入登录名对应的邮箱。
    * 输入Harbor project；此项为非必填。若您想将之后生成的镜像存放于Docker仓库里已有的project中，则在此填入对应的Harbor project名称即可。若不填，则默认在此仓库中新建一个Harbor project用于存放之后的镜像。
    * 点击测试连接，若连接成功，则代表自定义仓库有效；若连接失败，则无法使用。
    
> 此页面仅支持将默认的Docker仓库置为私有。

2. 修改默认Helm仓库为自定义Helm仓库。
    * 将默认Helm仓库切换为自定义Helm仓库。
    * 输入仓库地址。
    * 点击测试连接，若连接成功，则代表自定义仓库有效；若连接失败，则无法使用。


## 5. 阅读更多

- [测试设置](../test)
- [页面设置](../pages)