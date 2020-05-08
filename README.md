### 说明
go-sql-synchronize小工具，可以执行同步地方的相同数据库，异步执行，将执行之后的mysql返回的成功与失败结果显示
### 编译
> go build main.go
### 使用方法
> 在config/db.yaml 中添加需要同步的数据库连接
---
``` 
name: db_name
dsn: "db_user:db_password@tcp(db_link:3306)/db_table_name"
```     
> 在config目录下添加需要同步的sql语句
> 多个语句使用“;”分号隔开
