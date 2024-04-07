## DML
DML英文全称是Data Manipulation Language(数据操作语言)，用来对数据库中表的数据记录进行增、删、改操作。
### 添加数据
#### 给指定字段添加数据
```SQL
insert into employee(id,workno,name,gender,age,idcard,entrydate)values(1,'1','Itcast','男',10,'123456789012345678','2000-01-01');
```
#### 给全部字段添加数据
```SQL
insert into employee values(1,'1','Itcast','男',10,'123456789012345678','2000-01-01');
```
#### 批量添加数据
```SQL
insert into employee values(3,'3','韦一笑','男',38,'123456789012345670','2005-01-01'),(4,'4','赵敏','女',18,'123456789012345670','2005-01-01');
```
### 修改数据
```SQL
update employee set name = '小昭' , gender = '女' where id = 1;
```
### 删除数据
```SQL
delete from employee where gender = '女';
```
```SQL
delete from employee;