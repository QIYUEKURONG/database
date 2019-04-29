
# Go数据库的一些坑

## 关于open函数

这个函数需要一个driver。可以在 https://golang.org/s/sqldrivers 网站查看drivers的种类和去免费下载。
举个例子：
db，err：=open(drivername,root(database user):password@tcp(127.0.0.1(也可以是别的):port/databasename)
官方介绍：
Open may just validate its arguments without creating a connection to the database.
the Open function should be called just once. It is rarely necessary to close a DB.

## 关于

