# DBUtils

## 什么是DBUtils

### DBUtils是Apache公司编写的数据库操作实用的工具，小巧，简单，实用

### 封装了对JDBC的操作，简化了JDBC操作

## QueryRunner

### QueryRunner(DataSource ds)

- 提供数据源连接池，会自动帮你创建连接

### Update(String sql,Object...obj)

- 执行更新数据

### query(String sql, ResultSetHandler<T> rsh,Object...params)

- 执行查询

## ResultHandler

### query(sql, new BeanHandler<Student>(Student.class), params)

- 把查询的结果封装成一个指定对象

### query(sql, new BeanListHandler<Student>(Student.class)

- 把查询结果封装成一个指定对象集合

### qr.query(sql, new ScalarHandler())

- 查询单个值，返回为一个Long类型

### qr.query(sql, new MapListHandler())

- 把查询的结果封装成一个Map集合

### query(sql, new ColumnListHandler("列名"))

- 查询指定的列

*XMind: ZEN - Trial Version*