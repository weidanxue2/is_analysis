# 实验3：图书管理系统领域对象建模
|学号|班级|姓名|照片|
|:-------:|:-------------: | :----------:|:---:|
|201510414417|软件(本)15-4|魏丹雪|![flow1](../myself.jpg)|

## 1：图书管理系统的类图

### 1.1类图PlantUML源代码：
```
@startuml
package "Books Managerment System" #DDDDDD{
class Item {
  -create()
  -destroy()
  -find()
  -update()
  -find_on_reservation()
  -find_on_title()
}
class Title {
  -Create()
  -Find()
  -Destroy()
}
class Loan {
   -create()
    -destroy()
    -find()
    -pay()
}
class Reservation {
   -create()
    -destroy()
    -find()
}
class Manager{
     -create()
     -return_book()
     -maintain_borrower_message()
     -maintain_book_message()
 }
class Borrower {
   -create()
    -destroy()
    -find()
    -return_book()
    -check_if_max()
    -borrow_book()
    -modify_password()
}
Item "0..*" -- "1" Title:书籍标题管理
Reservation "0..*" -- "1" Title:预约书籍
Reservation "0..*" -- "1" Borrower:预约者信息
Loan "0..*" -- "1" Borrower:借阅读者信息
Loan "0..*" -- "1" Item:借阅书籍信息
Borrower "0..*" -- "1" Manager:维护读者信息
Item "0..*" -- "1" Manager:维护书籍信息

}
@enduml
```
### 1.2类图如下所示：
![](./system_class.png)
### 类图说明：
Title：标题类\
Ttem：书目类\
Reservation：预约类\
Borrower：借阅类\
Loan：借阅记录类
## 2：图书管理系统的对象图
### 2.1：类Item的对象图：
#### 源码如下所示：
#### 对象图如下所示：
### 2.2：类Reservation的对象图：
#### 源码如下所示：
#### 对象图如下所示：
### 2.3：类Borrower的对象图：
#### 源码如下所示：
#### 对象图如下所示：
### 2.4：类Title的对象图：
#### 源码如下所示：
#### 对象图如下所示：
### 2.5：类Reservation的对象图：
#### 源码如下所示：
#### 对象图如下所示：
### 2.6：类Loan的对象图：
#### 源码如下所示：
#### 对象图如下所示：
#### 2.7:系统的对象图：
#### 源码如下所示：
#### 对象图如下所示：
