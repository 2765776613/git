## 开源项目贡献流程

1. 新建issue

   提交使用问题或者建议或者想法

2. pull request 

   步骤：

   	1. fork项目
    	2. 修改自己仓库的项目代码
    	3. 新建pull request
    	4. 等待作者操作审核

## Git工作区域

1. 工作区：添加、编辑、修改文件等动作             
2. 暂存区：暂存修改的文件
3. Git仓库：最终确定的稳定保存到仓库，成为一个新的版本，并且对他人可见

```
工作区-->暂存区：
    git add hello.php
    git add test.php
暂存区-->Git仓库：
	git commit -m "提交描述"
```

**注意：git status  :   确定文件当前所处Git工作区域**

## Git初始化及仓库创建和操作

### 1. 基本信息设置

> 1. 设置用户名
>
>    git config --global user.name '2765776613'
>
> 2. 设置用户名邮箱
>
>    git config --global user.email '2765776613@qq.com'
>
> 3. 查看设置
>
>    git config --list

**注意**：该设置在github仓库主页显示谁提交了该文件

### 2. 初始化一个新的Git仓库

1. 创建文件夹

   > mkdir test

2. 在文件内初始化git（创建git仓库）

   > cd test
   >
   > git init  
### 3. 向仓库添加文件

   1. 创建一个文件

      > touch a1.php

   2. 添加到暂存区

      > git add a1.php

   3. 将文件从暂存区提交到Git仓库

      > git commit -m 'add a1.php'

### 4.  修改仓库文件

   1. 修改文件

      > vi a1.php

   2. 添加到暂存区

      > git add a1.php

   3. 将文件从暂存区提交到Git仓库

      > git commit -m '第一次通过git修改文件并提交到仓库'

### 5. 删除仓库文件

   1. 删除文件

      > rm a1.php

   2. 从git中删除文件

      > git rm a1.php

   3. 提交操作

      > git commit -m '第一次通过git删除仓库文件'

## Git管理远程仓库

### 1. 使用远程仓库的目的：备份，实现代码共享集中化管理

### 2. Git克隆操作

1. 目的：将远程仓库（github对应的项目）复制到本地

2. 代码：

   `git clone 仓库地址`

### 3. 将本地仓库同步到git远程仓库中

​		`git push`

## Github Pages 搭建网站

**个人站点：**	

1. 访问：https://用户名.github.io
2. 搭建步骤：

​	1）创建个人站点  ：  新建仓库（仓库名必须 是 【用户名.github.io】

​	2）在仓库下新建index.html的文件  ：  作为网站首页

**项目站点：**

1. 访问：https://用户名.github.io/仓库名

2. 搭建步骤：

   1） 进入项目主页，点击settings

   2） 在settings页面，点击【Launch automatic page generator】来自动生成主体页面

   3） 新建站点基础信息设置

   4） 选择主题

   5） 生成网页

   **注意：可在项目主页中的branches中的gh-pages目录下更改网页结构**



