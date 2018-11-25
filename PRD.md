# API_ML_AI
### Target release: 2019/01/01
### Epic:刷脸考勤

场景一：今天要上课的内容很多，这是一个很大的班，教秘那边又要求老师要给学生考勤，但无疑这会花去大量的时间。这时候通过人脸识别，轻松考勤，节约时间。


场景二：代课现象层出不穷，学校要求上课老师严打代课，可老师也不能保证能够精准的认出每个学生。这时候通过人脸识别，精准考勤，高效高质。
### Document Status: 未起头
### Document owner:朱凤
### Designer: 朱凤
### Developer: 朱凤
### QA: 朱凤
### Goals:
1.轻松考勤，节约时间，减轻老师的负担

2.精准考勤，高效高质，提高管理的质量
### Background and strategic fit:
目前的考勤方式主要是可以分为两种：全点和抽点
前者虽然相对全面，但因为学生基数大，需要花费大量的课堂时间，压缩课堂内容，这显然会影响教学效果。且及时是全点，也同样可能会遭遇代课代达到的情况。抽点虽然减少了点名的时间，但同样会出现也同样可能会遭遇代课代达到的情况，以及有所谓的幸运儿没到课但也没被发现的情况。针对这两困境，我们提出刷脸考勤，每个人的脸即便是双胞胎也不可能完全一样，这样可以有效的防止代课。其次自动识别自动考勤，减少考勤在课堂上时间的比重，有足够多时间完成教学任务。
### Assumptions: 
我们的用户主要以老师为主，通过电脑端进行操作，系统与课室摄像头相连接。用户可自行设置一个时间，达到之前所设置的时间之后课室的摄像头会自动拍摄一张当前课室的图片，然后识别人脸，与教务系统中选了该门课的学生的照片进行比对，符合的则登记到课，否则则为缺勤。
### Requirements: 
User story：石门中学已经全面启用人脸识别智能系统，届时学校正门、宿舍区域都会直接通过“刷脸”方式进出，“刷脸”1秒左右即可进出。“刷脸”系统还将记录学生请假、迟到等考勤情况。他们的刷脸是有固定机器需要特意去刷的，而我们这个是自己录像截图，自动识别，更加方便。

Title：刷脸考勤
### User interaction and design ：
默认页面：设置时间模块

通过输入数字来设定拍照时间

分析模块：后台分析

最后直接呈现给用户的是具体的考勤情况，设置一键导出的选项，将考勤导出成excel档；也可以云端累计考勤情况，期末再一键导出。

### Questions:是否会涉及到学生的隐私权问题

###  Not doing：自动将缺勤情况以短信形式发给家长