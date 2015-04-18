#My Homework
---
一个基于ExpressJs的Web应用，老师可以发布作业，学生可以提交作业  
使用nodeJs实现，数据库采用mongoDB


##功能
---
###教师
每个老师可以发布作业要求，并且只能看到自己发布的作业的要求。在作业页面，  
**老师既能看到学生提交的作业的情况，也能点击学生所提交作业以下载源文件**

More:  
1. 老师必须在deadline过后才能对学生的作业进行批改  
2. deadline未过时，即ddl大于当前时间，老师可以进行修改ddl和作业要求  

###学生
每个学生都可以看到所有作业的具体情况，并且能够查看自己作业的提交情况，也可  
以下载自己所提交的文件，并且能够查看自己作业所得分数

More:  
1. 只有在ddl之前才能够提交作业，可重复提交，以最后一次作业提交为准  

##HOW TO RUN
---
1. 命令行npm install
2. 运行mongod环境
3. 命令行运行grunt watch
4. 打开浏览器，localhost:5000

##HOW TO USE
---
1. 首次使用请先注册，并且选择您的身份(老师/学生)
2. 主页面左侧下拉列表为角色所拥有全部功能，主页默认查看所有作业，**若无，则不显示任何内容**
3. 学生提交的作业保存的文件夹路径为根目录下的homeworks，重新启动开发模式，文件不会被清楚
4. 学生上传文件必须按照格式 **userid + username.zip** 格式上传

##DEPENDENCIES
---
1. Node v0.12.1
2. ExpressJs v4.12
3. Mongoose
4. npm v2.5.1
