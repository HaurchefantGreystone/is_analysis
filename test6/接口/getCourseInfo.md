<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getCourseInfo  [返回](../README.md)
用例： [查看课程](../用例/查看课程.md)

- 功能：
    查看课程的所有信息。
    
- 权限：
    学生/老师：在登陆状态。    
    
- API请求地址： 
    接口基本地址/v1/api/getCourseInfo/<user_id>

- 请求方式 ：
    GET
      
- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |user_id|用户的ID号。对应表USERS.USER_ID的值|
  
- 返回实例：

        {         
            "status": true,
            "info": null,
            "id":"0000001"
            "name":"信息系统分析与设计"
            "semester":"2019-01"
            "teacher":null
            "student_num":0         
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |id|课程序号|
  |name|课名|  
  |semester|学期|
  |teacher|任课教师，null表示暂无教师任课|
  |student_num|选课学生数|

