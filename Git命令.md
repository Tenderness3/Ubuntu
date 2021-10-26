# Git命令
--------------------

### 克隆保存本地上传
>1、clone克隆
```python
$ git clone ...
...
...
$ git push
```


### 上传git步骤
>1、流程
```python
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
```

>2、添加子文件夹
```python
1、mkdir Text (创建文件夹，不用git init)
2、cd Text (进入文件夹)
3、touch 目标文件 (在子文件夹里面创建子文件夹)
4、cd .. (返回上一级目录)

开始上传流程
5、git add .
...
...
...
```



### git细节
>1、分支
```python
1、git status （查看当前状态）
2、git branch dev (建立分支dev)
3、git checkout dev (切换分支dev)
```


>2、查看以往commit
```python
1、git log
2、git log --oneline -6
3、git rflog（所有以往的版本）
4、git reset --hard HEAD~2 (返回过去第三行的版本)
```
>3、合并分支
```python
1、git merge dev（切换到master合并分支dev提供的版本）
2、git commit -m "merged by leader"（让领导选择---没有尝试）
```
>4、正确上传修改文件后缀名的步骤
```python
1、正常add
2、分别对不同文件commit
3、然后git push
```



### 解决错误
>1、解决冲突
```python
 1、git pull origin （查找github上层）
 2、git status （查看状态）
 3、按照提示操作删除
 4、git commit -m "发生冲突"  （提交这次冲突的变化）
 5、git push （上传）
 ```
>2、强制退出
```python
:q
```


