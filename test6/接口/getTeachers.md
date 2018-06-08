#### 用例： 老师列表
- 权限： 学生不能查看 、 老师登录后可以看到。
- 功能： 返回所有老师的列表。
- API请求地址： 接口基本地址/v1/api/getTeachers
- 请求方式 ： GET
- 请求参数说明: 无
```
 {
      "status": true,
      "info": "获取结果成功",
      "total": 25,
      "data": [
          {
          "GITHUB_ NAME": "Mr Zhao",
          "ID":19,
          "TCH_NO": 414213",
          "TCH_NAME": "赵老师",
          "STATUS":"1",
          "ADDTIME": "2018-05-22 17:48:01",
          "TERM_ID":2
          ...
          },
          
          {
          ...其他老师
          }
      ]
  }

```
- 返回参数说明：

参数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
total |返回老师人数
data | 所有老师的数组
GITHUB_ NAME | 	GITHUB 用户名
TCH_NO |实验编号
TERM_ID | 学期编号
TCH_NAME | 真实姓名
ADDTIME | 增加日期
ID | 数据库中编号
STATUS | 是否正常

