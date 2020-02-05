# PASS
 - 本網站稱為Programming Assignment Submission System(PASS)
    作為管理人員、教授、學生、TA間的溝通平台，幫助學生上傳作業，了解繳交狀況，幫助教授掌握作業進度，課程管理、幫助TA，批改作業，並且用圖形化的介面讓使用者更加方便管理。
    
## 目標
1.建置一個client-server 的網頁系統
2.利用本網站作為管理人員、教授、學生、TA間的溝通平台，
3.幫助學生繳交作業，了解繳交狀況，
4.幫助教授掌握作業進度，課程管理、
5.幫助TA，批改作業
6.用圖形化的介面讓使用者更加方便管理。


## 系統架構


本系統參考了北科開放式教室系統，以更簡化的使用方式完成此系統。

本系統共分為6個子系統︰
- 帳號管理子系統（User Account Management Subsystem, UAMS）
    - 負責管理所有帳號以及帳號使者權限。包含登入，帳號新增 、刪除、更改
- 課程管理子系統(Course Management Subsystem, CMS) 
    - 負責管理課程的新增、刪除修改。
- 作業管理子系統（Assignment Management Subsystem, AMS）
    - 負責管理作業的相關資訊。
- 作業繳交子系統（Assignment Submission Subsystem, ASS）
    - 能夠讓學生上傳作業，繳交完成後系統寄確認信。
- 繳交狀態追蹤子系統 （Submission Tracking Subsystem, STS）
    - 能夠查看作業繳交的狀態，並下載作業等。
- 報表子系統（Statistical Report Subsystem, SRS）
    - 根據課程或作業成績產生報表

### Asp.net  MVC 架構
![](https://i.imgur.com/TQDfNpt.png)

### 資料庫與檔案結構-ERModel

User(帳號資料): User_ID
Assignment(作業資料):  assignment_ID
Course(課程資料):Course_ID
- 關聯表:
    - Ta(助教): User_ID ，Course_ID
    - Elective(修課學生): User_ID ，Course_ID
    - Submit(繳交資料):User_ID，Assignment_ID

![](https://i.imgur.com/o23TlT8.png)

### 執行畫面



#### 登入
![](https://i.imgur.com/Gv7bXwv.png)

#### 個人頁面

![](https://i.imgur.com/uZPi91U.png)

#### 課程頁面
![](https://i.imgur.com/iZEBfVG.png)
#### 繳交作業
![](https://i.imgur.com/CMIyWmF.png)
#### 成績報表
![](https://i.imgur.com/NbFWzp5.jpg)
