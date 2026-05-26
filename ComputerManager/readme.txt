
企业资产管理系统(ComputerManage)

技术栈：FastAPI + SQLAlchemy 2.0 + MySQL + JWT
架构模式：Router->schema->model

项目优点：
    1.架构设计明确，模块分层，依赖注入且配置分离
    2.数据库设计，包括一对多，多对多和多层次外键等关系
    3.该项目为全异步，使用预加载selectinload数据库数据，避免N+1等情况，支持分页
    4.密码使用werkzeug.security哈希处理。登陆管理使用jwt认证，且项目包含权限控制，和字段验证，有较高的安全性
    5.该项目使用restful风格，可维护性高，包括类型注解、枚举管理、日志记录等，使用fastapi自动生成OpenAPI可预览测试。
