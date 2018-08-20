+++
title = "事务实例"
weight = 2
description = "实际运行的事务定义"
+++

# 事务实例

事务实例是实际运行的事务定义。一个事务定义可以有多个事务实例。

- **菜单层次**：全局层
- **菜单路径**：全局事务 > 事务实例
- **默认角色**：平台管理员

## 事务实例列表

事务实例列表展示了事务实例的基本信息。

- ID：事务实例的ID，是事务实例的标识，具有唯一性。
- 状态：事务实例的运行状态。共有`进行中`、`完成`、`失败`三种状态。
- 起始时间：事务实例开始运行的时间。以年-月-日 时:分:秒的形式展示。
- 终止时间：事务实例运行结束的时间。以年-月-日 时:分:秒的形式展示。
- 所属事务定义：实例所属的事务定义。一个事务定义下可以有多个实例。
- 关联业务类型：事务实例会关联至少一个业务。这个业务一般取事务实例运行时执行的第一个子事务所关联业务。业务有类型属性。该字段为事务实例关联的业务的业务类型。
- 关联业务ID：事务实例关联的业务的业务ID。

查看实例列表可以查看所有实例。选择查看失败实例，可以查看所有运行失败的实例，可以点击详情查看失败的具体情况并选择重试。

## 事务实例详情

- 点击事务实例列表的操作按钮→<img class="no-border" src="/docs/user-guide/system-configuration/global-transaction/image/particulars.png"/>可查看事务实例运行的详情。

- 详情页以图的形式展示实例的实际运行情况。图展示了按执行顺序执行的任务及输入、输出。

- 任务也可称为事务实例里的一系列子事务。任务一共有`等待`、`运行中`、`完成`、`失败`四种状态。

- 输入、输出为位于开始和结束节点的圆形。点击输入节点，显示json格式的输入参数的数据；点击输出参数，显示json格式的输出结果数据。

- 任务为位于输入、输出节点之间的正方形。点击任务节点，显示任务的运行情况和该任务在事件定义中的详情。 

- 任务的运行情况有如下信息：
     - 任务编码：用来标识任务，具有唯一性。
     - 状态：任务的状态，一共有`等待`、`运行中`、`完成`、`失败`四种状态。
     - 序列：任务在执行流程中的执行顺序。
     - 运行的微服务实例：运行这个任务的微服务实例。因为是分布式事务，所以不同的任务会分布在不同的微服务中运行。
     - 最大重试次数：若任务执行失败后，系统自动重试的最大次数。
     - 已重试次数：任务失败后，系统已经重试的次数。
     - 当状态为`完成`时，显示运行结果：显示json格式的输出结果数据。
     - 当状态为`失败`时，显示异常信息：导致任务运行失败的原因。

## 解锁任务

当任务的状态为等待、运行中或失败中任一种，且运行的微服务实例不为空时，任务将会被锁住，此时，允许进行解锁操作。

如果锁住任务的微服务实例出现异常，但任务没有接收到异常信息时，任务将保持锁住状态，此时，可以在界面将任务解锁，解锁后，任务可以被同一微服务的其他实例进行锁定。解锁步骤如下：

1. 点击事务实例的详情按钮→<img class="no-border" src="/docs/user-guide/system-configuration/global-transaction/image/particulars.png"/>。
1. 出现事务实例的事务执行流程图后，点击要解锁的任务。
1. 出现任务运行情况后，在运行情况底部点击解锁按钮→<img class="no-border" src="/docs/user-guide/system-configuration/global-transaction/image/unlock.png"/>。


## 重试任务

当任务的执行出现异常时，系统将会自动进行重试，当已重试次数达到最大重试次数的值时，该任务的状态将从运行中变为失败，允许用户可在界面上进行手动重试操作。重试步骤如下：

1. 点击事务实例的详情按钮→<img class="no-border" src="/docs/user-guide/system-configuration/global-transaction/image/particulars.png"/>。
1. 出现事务实例的事务执行流程图后，点击要重试的任务。
1. 出现任务运行情况后，在运行情况底部点击解锁按钮→<img class="no-border" src="/docs/user-guide/system-configuration/global-transaction/image/retry.png"/>。

## 更多操作
- [事务定义](../saga)