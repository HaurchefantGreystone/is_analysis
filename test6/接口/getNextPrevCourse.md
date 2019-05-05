<!-- markdownlint-disable MD033-->
<!-- 禁止MD033类型的警告 https://www.npmjs.com/package/markdownlint -->

# 接口：getNextPrevCourse  [返回](../README.md)
用例： [查看课程](../用例/查看课程.md)

- 功能：
    返回一个课程的上一个或者下一个课程的序号。
    
- 权限：    
    学生或教师在登陆状态。
    
- API请求地址： 
    接口基本地址/v1/api/getNextPrevCourse/<is_next>/<course_id>

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |is_next|是下一个还是上一个，如果为1表示取下一个学生，如果为0表示上一个学生|
  |course_id|学生的学号|
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "course_id": "0000001"
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |course_id|课程序号|

