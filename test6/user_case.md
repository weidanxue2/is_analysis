```
@startuml
:User: as Admin

Admin <|-- Teacher
Admin <|-- Student

:Admin: -up-> (修改密码)
:Admin: -up-> (修改用户信息)
:Admin: -up-> (查看用户信息)
:Admin: -up-> (登出)
:Admin: -up-> (登录)
:Admin: -up-> (选择学期)


:Teacher: -down-> (评定成绩)
:Teacher: -down-> (查看学生列表)
:Teacher: -down-> (选择教授课程)
:Teacher: -down-> (选择参考书籍)
:Teacher: -down-> (查看教学课程)

:Student: -down-> (查看自己的分数)
:Student: -down-> (查看成绩)
:Student: -down-> (选择自己的课程)
:Student: -down-> (查看所选课程)

@enduml
```
