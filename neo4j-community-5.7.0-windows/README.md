# 安装步骤
**1. 解压安装包**

**2. 进入系统属性设置环境变量**
以win10系统为例
* 打开电脑`高级系统设置`, 进入环境变量设置
  ![系统属性](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/20c1d024-d8e9-4d8f-8f62-d47c53bc6b79)
* 在系统变量处新建填写`NEO4J_HOME`，变量值填写压缩包的路径
  ![系统变量设置](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/fef34f0a-bd94-462a-ba79-248459f5b1fa)

  在环境变量处，点击Path，添加`%NEO4J_HOME%\bin`
  ![环境变量设置](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/a7ddcb0d-e291-49a5-8ef7-87fa2e4e0b89)

**3. 安装对应版本JDK**
  
  由于community 版本为5.7.0，顾选择JDK17，直接下载文件夹中 `jdk-17-windows-x64_bin.exe`文件
* 下载后双击安装即可
* 安装后，编辑path环境变量`%JAVA_HOME%\bin`
  ![编辑path环境变量](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/44d82099-3f44-480d-8cc2-730e516d3a0c)
* 新建系统变量`JAVA_HOME`
![新建系统变量](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/7c278c4b-e7bf-49fe-b2e0-705ed12d2b1f)


**4. 启动neo4j-community5.7.0**
  * 使用命令行语句键入代码`neo4j.bat console`，可以直接点击图中蓝线网址
    ![打开命令行输入命令](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/79d54d0c-3712-4b6f-8904-52d2fd310c59)

    ![打开蓝线网址](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/de7d0f36-39d0-4c4c-894b-87324c793c80)


  * 若想去警告
    
    想去掉这警告，可以直接打开community安装包中的`conf`文件夹的`neo4j.conf`文件（在解压包里，我的路径为D:\neo4j\neo4j-community-5.7.0-windows\conf）去掉最后一句代码`dbms.unmanaged_extension_classes=n10s.endpoint=/rdf`（这是当时我为了支持rdf格式导入新增的），或者改最后语句为`server.unmanaged_extension_classes=n10s.endpoint=/rdf`即可。
    ![d03c693e9cdddd298167192e71176c53](https://github.com/baixixi2020/Neo4j-5.7.0/assets/74234572/cdaa62f2-9551-408d-bab4-379e0af7d2bd)
