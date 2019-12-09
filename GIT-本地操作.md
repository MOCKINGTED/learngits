### 1. 创建
```
1.  项目的上一级目录中
git init
git config --global user.name "TED"
git config --global user.email "lhy19980302@163.com"

2. 项目的上一级目录中
git pull

3.  创建公钥加密，并取得公钥，填入GITHUB中
ssh-keygen
cat ~/.ssh/id_rsa.pub

4. 克隆项目
git clone git@github(github上有ssh的地址)

5. 进入项目地址
cd 项目
```

### 2. 一般步骤
```git
1. 将工作区文件加入暂存区
git add 文件名

2. 提交代码
git commit . -m "这是备注信息"

3. 上传到版本库
```

### 2. 比较
```git

比较工作区变动
git diff

工作区比较暂存区变动
git status

1. 暂存区与上一次版本库比较
git diff --cached 文件名

1.暂存区与指定记录比较
git log 		# 1. 找到指定hash值
git diff hash值 	# 2. 按照上面找到的hash值

暂存区与最新版本库比较
git diff HEAD

两个历史版本比较
git diff hash值1 hash值2
```

### 3. 忽略文件权限
```git
1. 当前版本库忽略文件权限信息
git config core.filemode false

2. 当前电脑的所有版本库忽略文件权限信息
git config --global core.fileMode false

3. 查看配置文件
cat .git/config

4. 如果配置文件中看到fileMode false表明配置成功
```

### 4.1 让git忽视文件
- `.gitignore`文件本身要放到版本库里面
1. 忽略自动生成的文件
2. 忽略编译生成的中间文件等一系列自动生成的文件
3. 忽略带有敏感信息的配置文件，比如存放口令的配置文件

```
1. 创建.gitignore文件
touch .gitignore
2. 将想要忽视的文件和名称加入，每行一个
.DS_store
.idea


```
### 4.2 让git添加回来忽视文件
```
1. 使用git命令控制
git check-ignore -v .DS_store

1. 使用强制添加
```

## 5 分支管理
- 上线使用`master`分支，开发用`develop`分支, 修改bug用`test`分支

### 5.1 查看分支
```
查看本地分支
git branch

查看本地和远程分支
git branch -a
```

### 5.2 新建分支
```
导入远程分支
git checkout master

1. 新建本地分支
git checkout -b 分支名
2. 指定远程分支名
git push --set-upstream origin 分支名
```

### 5.3 合并分支
```
将分支合并到master上
git merge test
```

### 5.4 删除分支
```
普通删除
git branch -d 分支名

强制删除
git branch -D 分支名
```