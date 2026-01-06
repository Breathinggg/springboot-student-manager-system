# 学生信息管理系统

> 2022年大学课程设计项目 - 基于 Spring Boot 的学生信息管理系统

## 项目简介

这是一个功能完整的学生信息管理系统，作为2022年大学期间的课程设计作品。系统支持三种用户角色：**学生**、**教师**、**管理员**。

## 功能模块

- **学生信息管理** - 学生的增删改查
- **教师信息管理** - 教师信息维护
- **班级信息管理** - 班级的管理
- **课程信息管理** - 课程的创建与管理
- **选课信息管理** - 学生选课功能
- **考勤信息管理** - 学生考勤记录
- **请假信息管理** - 请假申请与审批
- **成绩信息管理** - 成绩录入、导入导出、统计图表

## 技术栈

| 组件 | 技术 |
|------|------|
| 后端框架 | Spring Boot 2.0.1 |
| ORM | MyBatis |
| 模板引擎 | Thymeleaf |
| 前端UI | EasyUI |
| 数据库 | MySQL 5.5+ |
| 构建工具 | Maven |
| JDK | Java 1.8 |

## 快速开始

### 环境要求

- JDK 1.8
- MySQL 5.5+
- Maven 3.x

### 数据库配置

1. 创建数据库 `studentmanager`
2. 导入 `sql.sql`
3. 修改 `src/main/resources/application.yml` 中的数据库密码

```yaml
spring:
  datasource:
    url: jdbc:mysql://127.0.0.1:3306/studentmanager
    username: root
    password: 你的密码
```

### 运行项目

```bash
mvn clean install
mvn spring-boot:run
```

访问 http://localhost:8080

### 默认账户

| 角色 | 用户名 | 密码 |
|------|--------|------|
| 管理员 | admin | 123456 |
| 学生 | 王小明 | 123456 |
| 教师 | 赵老师 | 111 |

## 项目截图

<details>
<summary>点击查看截图</summary>

![登录页面](项目截图/1.png)
![主页](项目截图/2.png)
![学生列表](项目截图/3.png)

</details>

## 项目结构

```
src/main/java/com/wdd/studentmanager/
├── controller/     # 控制器
├── service/        # 业务逻辑层
├── mapper/         # MyBatis Mapper
├── domain/         # 实体类
├── config/         # 配置类
├── interceptors/   # 拦截器
└── util/           # 工具类
```

## License

本项目仅供学习参考。

---

*2022年大学课程设计作品*
