# 智慧图书管理系统

基于 Spring Boot、MyBatis-Plus、MySQL 和 Vue 的智慧图书管理系统，包含图书、读者、借阅订单、留言、收藏和论坛等功能。

## 技术栈

- Java 8 / Spring Boot 2.2.2
- MyBatis-Plus 2.3
- MySQL
- Vue 2 / Element UI

## 项目结构

```text
.
├── db.sql          # 数据库初始化脚本
└── zhihuitushu/    # Spring Boot 项目（含前端资源）
```

## 本地运行

1. 创建 MySQL 数据库 `zhihuitushu`，并导入 `db.sql`。
2. 按需设置数据库环境变量：

   ```bash
   export DB_URL='jdbc:mysql://127.0.0.1:3306/zhihuitushu?useUnicode=true&characterEncoding=utf-8&serverTimezone=GMT%2B8'
   export DB_USERNAME='root'
   export DB_PASSWORD='123456'
   ```

3. 启动后端：

   ```bash
   cd zhihuitushu
   mvn spring-boot:run
   ```

4. 访问 `http://localhost:8080/zhihuitushu/`。

示例管理员账号为 `admin`，密码为 `admin`。示例数据仅用于本地学习和演示，请勿用于生产环境。

