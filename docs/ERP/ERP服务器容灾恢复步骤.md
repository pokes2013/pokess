## 现状信息

1、数据库信息

MySQL版本：5.7.21

数据路径：D:\Mysql\mysql_x64\data\

问题：

Navcat自动备份的默认路径为：

```
C:\Users\Administrator\Documents\Navicat\MySQL\Servers\localhost_3308\s7
```

需要修改至E盘。或者脚本移动

E:\data_bak

命令行备份失败，原因是端口是3308

```
mysqldump -u root -p123456 s7 > "E:\data_bak\mydatabase_backup_%date:~0,4%%date:~5,2%%date:~8,2%.s
ql"
```

## 备份计划

- 自定义项
- 打印模版
- 基础数据
- 单据数据
- 正确的备份步骤

## 重新部署

- 打补丁之后，BOM才可修改
- 部署好之后必须激活才能登录
- 自定义项丢失
- 公式丢失
- 打印模版丢失

## 微调-自定义项

BOM供应商出不来

项目号料号出不来

## 细节的备份

公式的备份：截图备份位置，并且备份公式



## 自定义项的问题

注意：在BOM里面加的自定义项，公式要加在显示公式里面

BOM里面有4个自定义：

free1项目号

free2料号

free3客户代码

free4供应商

公式是调用存货档案，需要加再显示公式栏里面