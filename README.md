# MetaUni-Database
Contains docker-compose.yml to build database  
此文档帮助您使用Docker构建MetaUni项目中使用到的Database（目前包括MongoDB与SqlServer）  
阅读文档前请先确保：  
+ 您使用的操作系统为Windows
+ 您已顺利安装Docker Desktop  

以下条件不是必要，但可以显著增加您的体验：  
+ 您可以流畅访问外网 或 您已为Docker Desktop配置镜像源  

下面进入正题：  
1. 找一个合适的文件夹，将仓库内容拉取下来  
2. 打开CMD，`cd /d yourDir`，跳转至您存取仓库内容的文件夹  
3. 打开Docker Compose.txt文件，在CMD中依次输入文件内记录的命令（#后的命令为注释掉的内容，请跳过注释内容）
4. 检查Docker是否正确运行容器  

附：  
1.  MongoDB和SqlServer文件夹下的txt文件为单独启动MongoDB或SqlServer时所运行的命令，您可以选择遵照上文步骤使用`docker compose up -d`命令一次性启动所有容器，也可以选择依次运行单独启动容器的命令。  
2. Docker Compose.txt文件中记录的命令，从第二行开始便是在执行对MongoDB的设置操作，若先前已执行过操作，可忽略从第二行开始的内容。  
3. 执行完启动容器的命令后，MongoDB和SqlServer文件夹下会出现名字为“data”（或其它）的文件夹，这些文件夹用于与容器内部的文件进行关联（即Docker中的数据卷挂载，用于将部分重要数据持久化到宿主机中）。
