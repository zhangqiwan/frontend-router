## 创建GitHub项目

### 1. 创建GitHub账号和密码(远端)

待更新...

### 2. 下载git工具并配置（本地）

待更新...

### 3. 创建项目

- 登录GitHub远程仓库
- 进入自己的仓库Repositories
- 新建自己的项目仓库
  - 输入自己的项目/仓库名字——Repository name（必填）
  - 输入该项目/仓库的描述——Description（可选）
  - 输入项目类型——私有(private)还是公开(public)
  - 初始化设置：
    - Add a README file： 增加详细描述文件（建议勾选）
    - Add .gitignore: 增加git提交忽略文件， 其作用是助我们在git add时将我们指定的一些文件自动排除在外，不提交到git当中；（使用方式待补充）
    - Choose a license: 选择证书
  - 确认 Create repository

### 4. 更新项目到本地

- 进入创建的项目中， 获取项目的地址：git@github.com:zhangqiwan/frontend-router.git

  ![image-20210419001052742](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419001052742.png)

- 在本地git环境中使用：git clone git@github.com:zhangqiwan/frontend-router.git将仓库中数据更新到本地

  ![image-20210419001418098](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419001418098.png)

### 5. 更新项目到远程仓库

- 重要操作！重要操作！！重要操作！！！

  必须首先更新仓库中数据， 使用git pull <远程主机名> <远程分支名>  取回远程主机某个分支的更新，再与本地的指定分支合并

  ![image-20210419002846236](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419002846236.png)

  必须确保“Everything up-to-date”

- 先检查当前状态 status： git status

  ![image-20210419001638536](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419001638536.png)

  其中红色字体为修改的文件，并且在最后提示通过git add 将修改添加到提交列表中

- 然后新增 add：git add .   或者 git add xxx

  ![image-20210419001950283](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419001950283.png)

  ​	添加后通过git status查看状态， 发现文件新增成功

  ​	其中：

  	+ 如果你git status 查看了当前状态发现都是你修改过的文件，都要提交，那么你可以直接使用 git add .  就可以把你的内容全部添加到本地git缓存区中
  	+ 如果你git status 查看了当前状态发现有部分文件你不想提交，那么就使用git add xxx(上图中的红色文字的文件链接)  就可以提交部分文件到本地git缓存区。

- 再提交上传信息 commit： git commit -m "提交的信息"

  ![image-20210419002342650](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419002342650.png)

  git commit -m "提交代码"  推送修改到本地git库中

- 最后上传 push：git push <远程主机名> <远程分支名> 

  ![image-20210419002622271](D:\itproject\mygithub\frontend-router\GitHub\1-创建GitHub项目.assets\image-20210419002622271.png)

  把当前提交到git本地仓库的代码推送到远程主机的某个远程分之上

