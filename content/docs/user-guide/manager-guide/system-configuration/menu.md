+++
title = "菜单管理"
weight = 4
description = "用于配置平台菜单"
+++

# 菜单管理

## 概述

菜单管理用于配置平台菜单。进入平台管理、某一个组织、某一个项目、个人中心都需要菜单进行功能导航。因此，菜单配置按层级划分为全局层、组织层、项目层、用户层，且某一层级下只能配置相同层级的菜单
。您可以在此页面了解如何调整菜单顺序、创建目录、修改目录以及详情查看。

## 菜单管理列表

按菜单层级的方式查看菜单列表。一共分为 **平台**、**组织**、**项目**、**个人中心**，不同的层级对应不同的层级位置的菜单。

- 按**平台层**查看时，列表为用户在管理中心看到的菜单（默认该用户有平台层所有权限）；

- 按**组织层**查看时，列表为用户进入每一个组织看到的菜单（默认该用户有组织层所有权限）；

- 按**项目层**查看时，列表为用户进入每一个项目看到菜单（默认该用户有项目层所有权限）；

- 按**个人中心**查看时，列表为用户进入到个人中心的菜单。

列表字段：

- 目录/菜单：目录、菜单的名称。预置目录、菜单的名称无法修改，自设目录的名称可修改。

- 图标：目录、菜单的图标。预置目录、菜单的图标无法修改，自设目录的图标可修改。

- **编码**：目录、菜单的编码具有唯一性。

- 类型：分为目录、菜单和标签页三种，目录分为预置目录和自设目录两种。其中预置目录和菜单是系统定义的，用户无法修改，用户只能对自设目录进行创建、修改、删除。目录（包括预置目录和自设目录）和菜单为树型关系，菜单只能处于叶子位置，目录能处于根或分支的位置。

![列表](/docs/user-guide/manager-guide/image/menu-setting-01.png)

## 调整菜单顺序

您通过拖拽的方式，直接调整菜单的顺序和位置。

将鼠标移至列表字段目录/菜单，会显示一个虚线框，该虚线框内则为鼠标长按拖动时可拖动的内容。如果一个目录下没有菜单，则不显示该目录。

如果鼠标悬停在目录上，虚线框内则为此目录和该目录下的所有目录/菜单，鼠标长按时可拖动此目录和该目录下的所有目录/菜单；若该目录下无目录/菜单，则虚线框内只有这个目录，鼠标长按时只可拖动这个目录。

如果鼠标悬停在菜单上，虚线框内只有这个菜单，鼠标长按只可拖动这个菜单。

## 创建目录

1. 点击工具栏上方的`创建目录`，创建一个新目录。
2. 在创建页面中填写目录编码、名称，再选择图标，
    必填字段：
    - 目录名称：用户可根据需要自定义名称。
    - 目录编码：目录编码具有唯一性，是目录的标识。
    - 目录图标：目录的图标可在系统提供的图标库中选择。

3. 点击添加即可完成。

![列表](/docs/user-guide/manager-guide/image/menu-setting-02.png)


## 修改目录

1. 点击目录行中的![三点](/docs/user-guide/manager-guide/image/more-vert.png)标识，点击`修改目录`，进入修改页面。

    可修改字段：
    - 目录名称：目录的名称，根据需要自定义名称。
    - 图标：目录的图标，在系统提供的图标库中选择。

    不可修改字段：
    - 目录编码：具有唯一性，是目录的标识。所以目录一旦成功创建，不可修改。
2. 点击`保存`，保存对自定义目录的修改。

## 查看详情

点击菜单行中的![三点](/docs/user-guide/manager-guide/image/more-vert.png)按钮，点击`查看详情`，可查看菜单的菜单名称、菜单编码、菜单层级、所属根目录和菜单所具有权限。

> 详情字段：

> 菜单名称：菜单的名称，根据菜单功能定义菜单名称。

> 菜单编码：菜单编码具有唯一性，是菜单的标识。

> 菜单层级：菜单有层级性，只能在相同的层级配置菜单。例如，在项目层只能配置菜单层级为项目层的菜单。

> 所属根目录：一个菜单必须且只能属于一个目录。

> 菜单权限：要实现菜单里所有功能需要的权限。

## 删除自设目录

点击列表中![三点](/docs/user-guide/manager-guide/image/more-vert.png)标识选择`删除目录`按钮，删除自设目录。

<blockquote class="warning">
         只有自设目录可删除，预置目录和菜单不可是系统定义的，无法删除。
      </blockquote>

如果目录下有菜单，则不可删除该目录；只有当目录下无菜单时，可删除该目录。例如，在一个目录A下有目录B，目录A可以被删除；在一个目录C下有目录D，目录D下有菜单1、菜单2，目录C、目录D不可被删除。

##  阅读更多
- [角色管理](../role)
- [用户管理](../site-user)
- [通用设置](../site-setting)
