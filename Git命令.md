## Git命令
============

## 克隆保存在本地和上传
$ git clone ...
...
...
$ git push


## 上传git步骤
~~~bash
1、git init（初始化git）
2、git add . (添加到暂存区)
3、git reset HEAD index.html (取消暂存区绿色的内容，不更改内容)
	git checkout -- index.html(--后面有空格就是恢复上一次修改，就是add后变红了，然后取消变红，不要轻易使用)
4、git commit -m "注释" （添加到本地数据库）

5、git commit --amend （假如想覆盖上次上传
	1、直接add
	2、然后输入git commit --amend会进入一个特殊的场景，展示修改本地数据库文件
	3、修改后既可以git push）
6、git push （上传到github服务器）
~~~
## git细节
~~~bash
1、git status （查看当前状态）
2、git branch dev (建立分支dev)
3、git checkout dev (切换分支dev)
4、git log
5、git log --oneline -6
6、git rflog（所有以往的版本）
7、git reset --hard HEAD~2 (返回过去第三行的版本)


1、git merge dev（切换到master合并分支dev提供的版本）
2、git commit -m "merged by leader"（让领导选择---没有尝试）
~~~

## 解决冲突
~~~bash
 git pull origin （查找github上层）
 git status （查看状态）
 按照提示操作删除
 git commit -m "发生冲突"  （提交这次冲突的变化）
 git push （上传）
 
 ~~~


