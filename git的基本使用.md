### 克隆一个git仓库到本地 然后添加远程仓库
1. 在github上创建一个远程仓库note 
2. 生产ssh秘钥 
```
ssh-keygen -t rsa -C "17674755974@163.com" 
```
3. 将cd到 ~/.ssh 将文件夹下的 id_rsa.pub 里面的内容拷贝到github的ssh认证里面
4. 在本地的一个文件夹下克隆远程仓库
```
git clone git@github.com:jianJizz/note.git
```
5. 这个时候就关联了远程仓库使用git remote -v 可以看到所有关联的远程仓库地址及别名
6. 关联远程仓库
```
git remote add note git@github.com:jianJizz/note.git
```
7. 可以删除原来关联的note.git git remote rm origin(关联的远程仓库的别名)
8. 推送数据到远程仓库
```
git push note master
```
9. gitnote github图床的使用 按照官网给的步骤在github上配置 然后截张图复制即可自动上传 在设置里还可以自己选择默认图床
![title](https://raw.githubusercontent.com/jianJizz/gitnote-images/master/gitnote/2019/05/01/1556648610629-1556648610631.png)
10. git 提交代码 
```
git add . 提交当前目录下的所有到工作区
git commit -m ‘desc’ 提交代码到git
git push coding master 提交到远程仓库的master分支
```
