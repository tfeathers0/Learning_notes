> 教程资源
>
> [lec2 - 2023春夏实用技能拾遗](https://slides.tonycrane.cc/PracticalSkillsTutorial/2023-spring-cs/lec2/#/3/4)

# Git 基础配置

![image-20240822115539384](C:\Users\33071\AppData\Roaming\Typora\typora-user-images\image-20240822115539384.png)（需要修改）

* 
  创建一个本地版本库
  * 'git init' 
    * git init: 让当前文件夹变成git仓库 (创建 .git文件夹)
    * git init folder:
* git账号配置
  * git config --global user.name "name"
  * git config --global user.email "email"
    * 区分用户 / 让GitHub识别
    * 全局配置
    * 针对某一版本库专门设置
      * 同前, 不加--global


# Git基础用法

## 文件暂存

* 将文件加入暂存区stage中
  * git add file/folder
    * 只会添加修改过的文件	
* 删除文件
  * rm
    * 只在本地删除版本库commit history中不存在的文件
  * git rm
    * 同时删除本地和版本库中的文件
    * 相当于先rm, 再add
  * git rm --cached
    * 将一个一暂存的新文件取消暂存
* 重命名文件
  * git mv
    * 等价于mv + git rm + git add
* 查看当前工作区和暂存区状态
  * git status
    * Untracked \ Tracked \ Igonored

## .gitigonore❓

- 存放在版本库根目录下的名为 .gitignore 的文件，规定忽略哪些文件
- 语法
  - \# 开头的行为注释
  - \* 通配多个字符，** 通配中间目录（有或无）
    - *.c 匹配所有 C 文件，a/**/b 匹配 a/b、a/x/b、a/x/y/b 等
  - / 开头只匹配根目录，否则匹配所有目录
  - ! 取消忽略
  - ...
  - [Git - gitignore Documentation](https://git-scm.com/docs/gitignore)
- git check-ignore -v *file*：查看某个文件是否被忽略，以及匹配的规则
- 常用语言的 .gitignore 模板：[github/gitignore](https://github.com/github/gitignore)

## 提交更改

* 将暂存stage中的内容提交到本地仓库 (本质上是一个提交历史), 生成一个新版本

  * git commit
    * 默认编辑器编辑提交信息
    * -m "message"
    * -a | --all: 自动暂存所有更改的文件

* 查看提交历史

  * git log
    * --oneline: 每一个提交一行
    * --graph: 显示分支结构
    * --stat: 显示文件删改信息
    * -p: 显示详细的修改内容

* 显示提交详细信息

  * git show id: 显示提交详细信息 (id不重复前提下可以只写前几位)

>  每个提交都有唯一的sha-1标识符 (40位16进制数)

* 检出之前的某一版本

  * git checkout id

## 关于commit message

- 意义是什么：记录更改的原因 / 内容，方便定位 / 回溯（特别是合作项目）

- Angular 规范（来源：[angular/angular:CONTRIBUTING.md](https://github.com/angular/angular/blob/main/CONTRIBUTING.md#-commit-message-format)）

  ```
  <type>([scope]): <summary>
  
  [body]
  
  [footer]
  ```

  - type：更改类型（fix/feat/docs/refactor/perf/test/ci/...）
    - 重大更改可以写 BREAKING CHANGE 或 DEPRECATED（全大写）
  - scope：影响范围（可选，比如具体影响的模块等）
  - summary：更改的简要描述，英文一般现在时，首字母小写句末无句号
  - body：详细描述，可选
  - footer：解决 issue 了可以写 Fixes #*id* 或 Closes #*id*

## 关于版本

- 创建标签：
  - git tag *tag* *id*
    - 轻量标签
    - *id* 可选，默认为 HEAD
  - git tag -a *tag* -m "*message*" *id*
    - 附注标签
- 查看标签
  - git tag
- 版本号命名一般规范：Semantic Versioning 2.0.0
  - v*主版本号*.*次版本号*.*修订号*[-*预发布版本号*]
  - 修订号：兼容修改，修正不正确的行为
  - 次版本号：添加新功能，但是保持兼容
  - 主版本号：不兼容的API修改
    - 且为 0 时表示还在开发阶段，不保证稳定性
  - 预发布版本号：alpha/beta/rc.1/rc.2/...
  - e.g. v1.0.0-beta < v1.0.0-rc.1 < v1.0.0 < v1.0.1

> git diff A B(分别对应ab, a用- ,b用+,最好设置A为旧文件,B为新文件)
