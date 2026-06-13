![[Pasted image 20260613161630.png|697]]
![[Pasted image 20260613161725.png]]
![[Pasted image 20260613161740.png]]
MYSQL数据类型主要分为三类：数值类型、字符串类型、日期时间型。
![[Pasted image 20260613162042.png]]
age年龄没有复数所以用unsigned
score double(4,1)4代表数字长度，1代表小数点后一位
![[Pasted image 20260613162238.png]]
带blob是二进制数据带text是带文本的数据
括号内代表当前字符串储存的最大长度
char（10）：定长字符串，即使只存储1个字符也会占用10个字符的空间，其它空间会使用空格进行补位-----性能好
vatchar（10）：会根究你当前存储的内容去计算当前所占用的空间多打-----性能较差
举例：用户名 usename varchar（50）用户名长度不确定所以用变长
       性别   gender char（1）    
    ![[Pasted image 20260613163344.png]]
birthday date生日一般记录年月日
![[Pasted image 20260613163616.png]]
CREATE TABLE emp (
    id INT COMMENT '编号',
    workno VARCHAR(10) COMMENT '工号',
    name VARCHAR(10) COMMENT '姓名',
    gender CHAR(1) COMMENT '性别',
    age TINYINT UNSIGNED COMMENT '年龄',
    idcard CHAR(18) COMMENT '身份证号',
    entrydate DATE COMMENT '入职时间'
) COMMENT '员工表';

![[Pasted image 20260613165718.png]]
![[Pasted image 20260613165740.png]]
![[Pasted image 20260613170118.png]]
![[Pasted image 20260613170225.png]]
![[Pasted image 20260613170409.png]]
