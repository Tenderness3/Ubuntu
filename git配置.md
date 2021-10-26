# Git 配置
--------
### git登录配置
>1、配置用户名、邮箱
```python
1、git config --global user.name "Tenderness3
2、git config --global user.email "1360379591@qq.com"
3、git config -l  (查看配置信息)
```
>2、配置ssh密匙
```python
ssh-keygen -t rsa -C "1360379591@qq.com"
```
>3、检测是否连接上
```python
1、ssh -T git@github.com
2、yes
```
>4、克隆
```python
git@github.com:Tenderness3/Ubuntu.git
```
>5、解决git bash 中文变成数字问题
```python
git config --global core.quotepath false
git status (查看状态)
```
>5、在该文件的.git下添加  gitee
```python
url = git@gitee.com:liu-rushi/ubuntu.git
git remote -v （查看当前仓库信息）
未配置成功！！！！！
```