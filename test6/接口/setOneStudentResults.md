#### 用例： 评定成绩
- 权限：老师登录后可以查看
- 功能：  设置一个学生的部分实验成绩和评语。    
- API请求地址： 接口基本地址/v1/api/setOneStudentResults
- 请求方式 ： post
- 请求实例：

```
  {         
      "STU_NO": "201510414206", 
      "GITHUN_NAME": "HuangShengqi", 
      "STU_CLASS": "软件(本)15-2", 
      "STU_NAME": "黄长生", 
      "data": [
          {
          "GRADE_ID":1,
          "TEST_ID": "51", 
          "COURSE_NO": "41051", 
          "STU_NO":"201510414213",
          "GRADE_1":95,
          "GRADE_2":94,
          "GRADE_3":91,
          "MOME":"本实验做得一般",
          }
      ] 
  }

```
- 请求参数说明：

	数名称	| 说明
---|---
STU_NO |学生编号
GITHUN_NAME |GITHUB用户名
STU_CLASS |学生班级
STU_NAME |学生姓名
total |返回记录
data |返回结果的数组
GRADE_ID| 分数编号
TEST_ID |实验编号
COURSE_NO |课程编号
STU_NO |学生编号
GRADE_1 |分数1
GRADE_2 |分数2
GRADE_3 |分数3
MOME |评价


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


