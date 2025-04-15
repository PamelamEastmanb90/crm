# 雨云MCSM面板搭建Minecraft Forge 1.20.2服务器全流程指南

## 雨云游戏云核心优势

雨云面板服支持一键开服的游戏包括：
- Minecraft Java版/基岩版
- 泰拉瑞亚
- 饥荒
- 纯Java/Linux环境（Docker）

针对Minecraft Java版，已预置多种服务端支持：
✔ Arclight ✔ Mohist ✔ CatServer  
✔ SpongeForge ✔ Fabric ✔ BungeeCore  
（注：Forge需通过纯Java环境手动搭建）

👉 [【点击查看】2025年最新雨云优惠码及特价云服务器方案汇总](https://bit.ly/RainYun)

## 硬件配置方案

### 专业级游戏云配置
- **CPU方案**：
  - i9-13900K 5.8GHz
  - Ryzen9 5900X 4.8GHz
  - Xeon Gold 6146 4.2GHz
- DDR4高频内存
- NVMe SSD存储阵列

## 服务模式对比

### VPS专业版
- 基于KVM虚拟化技术
- 支持Windows/Linux双系统
- 15个开放端口
- 多服务端并行部署

### 面板服便捷版
- MCSM/翼龙面板管理
- 按日计费（最低0.5元/天）
- 网页端全功能操作
- 新手友好型控制台

## Forge服务端部署教程

### 环境准备
1. 注册雨云账号
2. 控制台选择【游戏云】→【MCSM面板】
3. 选择【纯Java环境】
   - 1.16.5以下：Java8
   - 1.16.5：Java11
   - 1.17+：Java17

### 服务端配置
bash
# 典型启动参数示例
java -Xms128M -XX:MaxRAMPercentage=95.0 
     -Dfile.encoding=UTF-8 
     -Duser.language=zh 
     -Duser.country=CN 
     -jar forge-1.20.2-48.0.30-installer.jar

### 关键配置项
1. 修改`eula.txt`确认用户协议
2. 调整`server.properties`：
   - online-mode=false（关闭正版验证）
   - server-port=自定义端口

## 玩家连接指南
1. 获取服务器地址（控制台显示）
2. 格式：`域名:端口`
3. 客户端需安装对应版本Forge

## 运维管理技巧
- 动态资源监控
- 自动备份系统
- 实时性能调整
- 多实例集群管理

> 小贴士：建议4核8G以上配置运行高版本Mod服，遇到技术问题可查阅雨云知识库文档