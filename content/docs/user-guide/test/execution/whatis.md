+++
title = "什么是测试执行"
description = ""
weight = 1
+++

# 什么是测试执行

## 1. 概述

执行测试即为测试运行或执行时发生的事情提供一个高级的状态，并对其进行一些后续操作。

执行可以对测试用例进行执行，可以跟踪进度并提供质量度量的报表。

## 2. 为什么用测试执行

使用测试执行可以：

- 提高测试的灵活性和规范性
- 并且提高测试用例的复用性
- 最终达到减少测试时间的目的

## 3. 查看测试执行

通过`测试用例树`选择你想要查看的测试循环或阶段，层级逻辑为：版本对应的状态>版本>测试循环>测试阶段。

- 循环和阶段名称右边会显示目前的测试执行进度。
- 在测试用例树上方可以选择`我的执行`和`所有执行`，或者直接搜索来显示出想要的测试用例。

![image](/docs/user-guide/test/execution/image/TestExecute-02.png)


## 4. 查看测试执行进度

您可以在测试用例列表上方查看某循环或某阶段的当前执行进度。

包括：测试之心进度条、版本、开始时间和结束时间、创建人、构建号、环境、说明。

![image](/docs/user-guide/test/execution/image/TestExecute-03.png)

## 5. 查看测试用例

测试用例列表显示的是对应测试循环和测试阶段的测试用例。

展示字段包括：用例名称、执行方、被指定人、阶段名称、优先级、状态。

![image](/docs/user-guide/test/execution/image/TestExecute-04.png)

其他操作：

- 点击用例行最右的![image](/docs/user-guide/test/execution/image/TestExecute-07.png)，可以切换通过或失败的状态。
- 点击快速筛选处的下拉菜单`执行方`和`被指定人`可以对用例进行筛选。

## 6.  阅读更多

- [创建测试用例](../../store/create)
- [管理测试用例](../../store/manage)
- [执行测试](../../execution/)