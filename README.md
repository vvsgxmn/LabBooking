# 基于SpringBoot+Vue的实验室预约系统

![Spring Boot](https://img.shields.io/badge/-Spring%20Boot-6DB33F?style=flat-square&logo=spring-boot&logoColor=white) ![Vue3](https://img.shields.io/badge/-Vue3-grey?style=flat-square) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![MyBatis](https://img.shields.io/badge/-MyBatis-000000?style=flat-square&logo=mybatis&logoColor=white) 

## 项目介绍

本系统是一款面向高校师生与实验中心管理员的智慧实验室预约与资源共享平台，针对实验工位冲突、仪器借还难追溯、耗材账实不一致、安全准入难核验等痛点，将实验空间预约、精密仪器借用、耗材申领、安全准入考核与故障报修整合到同一门户，支撑从申请提交到审批履约的完整闭环。

系统采用 SpringBoot + Vue 前后端分离架构，区分普通师生与系统管理员：师生端完成实验室浏览预约、仪器借用、耗材申领、安全考试、故障报修与个人中心查询；管理员在数据看板审核预约/借用/申领、维护实验室与设备耗材台账、管理安全题库与用户审核启用。适合作为毕设、课设与高校实验资源数字化学习参考。

## 主要功能模块

- **用户认证与注册审核**：师生注册后待管理员审核启用方可登录；JWT 鉴权，USER/ADMIN 双角色分流
- **实验空间预约**：按学科分类浏览实验室，选择日期时段与人数提交预约，支持签到签退与进度查询
- **精密仪器借用**：查看设备可用量与使用指南，提交借用起止日期，审批通过后扣减可用台数，归还后回补
- **实验耗材申领**：库存与预警提示，填写用途与数量提交申领，管理员审批发放
- **安全准入考核**：在线题库答题，达标后获得准入资格，高危实验室可强制要求持证预约
- **设备故障报修**：选择实验室与故障设备，上传现场照片提交工单，跟踪维修反馈
- **通知规章与个人中心**：浏览公告资讯，查看我的预约/借用/申领/报修记录并维护个人资料
- **管理数据看板**：ECharts 展示预约、设备与资源运营指标
- **资源台账中台**：学科分类、实验室档案、仪器设备、耗材库存与公告维护
- **审批与运维**：预约审批、借用审核、申领审批、故障工单处理、安全题库与用户启用禁用

## 技术架构

- **后端**：Spring Boot 2.7 + MyBatis-Plus + JWT + Lombok
- **前端**：Vue 3 + TypeScript + Vue Router + Pinia + Element Plus + Vite + ECharts
- **数据库**：MySQL 8.0

<!-- screenshots-start -->
## 系统截图

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E7%99%BB%E5%BD%95%E9%A1%B5%E9%9D%A2.png" alt="登录页面" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E7%94%A8%E6%88%B7%E9%A6%96%E9%A1%B5.png" alt="用户首页" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E5%AE%9E%E9%AA%8C%E7%A9%BA%E9%97%B4.png" alt="实验空间" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E4%BB%AA%E5%99%A8%E5%80%9F%E7%94%A8.png" alt="仪器借用" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E5%AE%89%E5%85%A8%E5%87%86%E5%85%A5.png" alt="安全准入" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E7%AE%A1%E7%90%86%E5%91%98%E6%95%B0%E6%8D%AE%E7%9C%8B%E6%9D%BF.png" alt="管理员数据看板" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E5%90%8E%E5%8F%B0%E9%A2%84%E7%BA%A6%E5%AE%A1%E6%89%B9.png" alt="后台预约审批" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E5%90%8E%E5%8F%B0%E5%AE%9E%E9%AA%8C%E8%80%97%E6%9D%90.png" alt="后台实验耗材" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E8%AE%BA%E6%96%87%E5%9B%BE1.png" alt="论文图1" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/%E8%AE%BA%E6%96%87%E5%9B%BE2.png" alt="论文图2" width="600" />

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/AutoUpload/screenshots/labbooking/UML%E5%9B%BE%E5%88%97%E8%A1%A8.png" alt="UML图列表" width="600" />

<!-- screenshots-end -->

---

## 接毕业设计和论文

### 作者微信：vvsgxmn  (支持修改、 部署调试、 支持代做毕设)

### 接网站建设、小程序

### 选题+开题报告+任务书+程序定制+安装调试+论文+答辩ppt 都可以做

### 购买地址：[https://www.vvxx.love](https://www.vvxx.love)（vv毕设网）

### 支持 **一键生成 UML 图**：上传项目压缩包即可自动产出功能模块图、用例图、流程图、E-R 图、时序图等全套毕设图表。

### 提供 **免费配套软件下载 + 安装说明 + 部署教程**

![vv毕设网 - 一键画图](https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/uml-draw.png)

<img src="https://fanhua-yingcai.oss-cn-shanghai.aliyuncs.com/image-20260825133349317.png" alt="image-20260825133349317" />

⚠️ Bug添加微信**免费修复**，免费修复。其他平台的私信一律不管（微信方便发送文件）
