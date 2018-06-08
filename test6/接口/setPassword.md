#### 用例： 修改密码
- 权限：学生/老师：修改自己的密码，必须先登录。
- 功能： 修改（设置）用户的密码。    
- API请求地址： 接口基本地址/v1/api/setPassword/<type>
- 请求方式 ： post
- 请求实例：

```
  {         
      "TYPE":"stu",
      "no":"201510414206"
      "password":AF#W@#AAAASDF
  }

```
- 请求参数说明：

	数名称	| 说明
---|---
TYPE |类别
no |学号
password |密码


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


