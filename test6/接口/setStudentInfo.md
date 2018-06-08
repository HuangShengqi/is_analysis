#### 用例： 修改学生信息
- 权限：学生/老师：修改自己的密码，必须先登录。
- 功能： 修改学生的基本信息。
- API请求地址： 接口基本地址/v1/api/setPassword/<stu_no>
- 请求方式 ： post
- 请求实例：

```
  {         
      "stu_no":"201510414206",
      "data": 
          {
          "GITHUB_ NAME": "HuangShengqi",
          "ID":15,
          "STU_NO": "201510414206",
          "STU_CLASS": "软件(本)15-2",
          "STU_NAME": "黄长生",
          "STATUS":"1",
          "ADDTIME": "2018-05-22 17:48:01",
          ...
          }
  }

```
- 请求参数说明：

	数名称	| 说明
---|---
stu_no|学生学号
data | 学生信息集合
ID |数据库自增
	ITHUB_ NAME | 	GITHUB 用户名
STU_NO | 学号
STU_CLASS| 班级
STATUS|是否正常
STU_NAME | 真实姓名
ADDTIME | 增加日期

- 返回实例：
```
{         
      "status": true,
      "info": "修改成功"
  }
```


参数名称 | 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息


