### 克隆一个git仓库到本地 然后添加远程仓库
1. 在github上创建一个远程仓库note 
2. 生产ssh秘钥 
```
ssh-keygen -t rsa -C "17674755974@163.com" 
```
3. 将cd到 ~/.ssh 将文件夹下的 id_rsa.pub 里面的内容拷贝到github的ssh认证里面
4. 在本地的一个克隆远程仓库
```
git clone git@github.com:jianJizz/note.git
```
5. 这个时候就关联了远程仓库
