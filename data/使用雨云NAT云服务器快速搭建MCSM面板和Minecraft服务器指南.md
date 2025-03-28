# 使用雨云NAT云服务器快速搭建MCSM面板和Minecraft服务器指南

## 前言：端口映射与服务器配置基础

端口映射是搭建Minecraft服务器的关键步骤，虽然对新手来说可能有些复杂，但通过本教程的详细指导，您将能够轻松掌握这项技能。以下是分步操作指南：

## 详细配置步骤

### 第一步：创建端口映射规则

1. **设置内网端口**：
   - 选择需要公开的内部网络端口
   - 点击"创建映射规则"完成操作
   - 系统会自动处理外部端口分配

> 提示：如果默认端口被占用，可选择任意空闲端口替代

### 第二步：配置节点与更新设置

1. **节点配置**：
   - 选择适用的服务器管理软件
   - 设置节点地址为服务器IP或域名
   - 将端口参数调整为24444映射至公网端口
   - 点击"更新"按钮保存设置

👉 [【点击查看】2025年最新雨云优惠码及特价云服务器方案汇总](https://bit.ly/RainYun)

### 第三步：编辑Web面板服务

bash
nano /etc///mcsm-web.

1. 按示例输入需要修改的信息
2. 使用`Ctrl+O`保存更改
3. 使用`Ctrl+X`退出编辑界面

### 第四步：修改配置与添加密钥

- 将"127.0.0.1"替换为服务器公网IP或域名
- 调整外部应用的24444端口号
- 执行以下命令下载所需插件：

bash
java -Xmx4G -Dfile.=UTF-8 -Duser.=zh -Duser.=CN -jar ${}

### 第五步：解析启动命令

- 严格遵循"-Xmx4G"参数设置内存限制
- 可根据服务器配置适当增加内存
- 检查全局配置：

bash
cat /opt/mcsmanager/daemon/data/Config/global.json

### 第六步：启动实例与EULA协议

1. 点击"启动实例"按钮
2. 阅读并接受EULA协议
3. 输入"true"进行确认

### 第七步：服务器最终设置

- 前往"相关设置→【通用】界面
- 根据实际情况调整服务器参数
- 非正版用户需关闭正版验证
- 点击"保存"完成设置

## 结语

通过以上七个步骤，您已成功在雨云NAT服务器上搭建了MCSM面板和Minecraft服务器。如有任何疑问或独特的管理经验，欢迎分享交流！