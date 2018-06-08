#### 用例： 学期列表
- 权限： 学生/登录后可以看到。
- 功能： 返回所有学期的列表。
- API请求地址： 接口基本地址/v1/api/getTerms
- 请求方式 ： GET
- 请求参数说明: 无
```
 {
      "status": true,
      "info": "获取结果成功",
      "total": 8,
      "data": [
          {
          "TERMS_ID":19,
          "TITLE": 大三下学期",
          "ADDTIME": "2018-05-22 17:48:01",
          ...
          },
          
          {
          ...其他学期
          }
      ]
  }

```
- 返回参数说明：

参数名称	| 说明
---|---
status | bool类型，true表示正确的返回，false表示有错误
info | 返回结果说明信息
total |返回学期数量
data | 所有学期的数组
TERMS_ID | 	学期编号
TITLE |学期名称
ADDTIME | 增加日期


