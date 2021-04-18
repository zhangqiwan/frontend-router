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

- 先检查当前状态
- 然后新增 add
- 再提交上传信息 commit
- 最后上传 push