### 1. 创建
```
// 1.  项目的上一级目录中
git init
git config --global user.name "TED"
git config --global user.email "lhy19980302@163.com"

// 2. 项目的上一级目录中
git pull

// 3.  创建公钥加密，并取得公钥，填入GITHUB中
ssh-keygen
cat ~/.ssh/id_rsa.pub

//  4. 克隆项目
git clone git@github(github上有ssh的地址)

// 5. 进入项目地址
cd 项目
```git
### 2. 一般步骤
```git
// 1. 将工作区文件加入暂存区
git add 文件名

// 2. 提交代码
git commit . -m "这是备注信息"

// 3. 上传到版本库
```

### 2. 比较
```git

//  1. 比较工作区变动
git diff

//  2. 工作区比较暂存区变动
git status

// 3. 暂存区与上一次版本库比较
git diff --cached 文件名

// 4.暂存区与指定记录比较
git log 		# 1. 找到指定hash值
git diff hash值 	# 2. 按照上面找到的hash值

// 5. 暂存区与最新版本库比较
git diff HEAD

// 6. 两个历史版本比较
git diff hash值1 hash值2
```

### 3. 忽略文件权限
```git
// 1. 当前版本库忽略文件权限信息
git config core.filemode false

// 2. 当前电脑的所有版本库忽略文件权限信息
git config --global core.fileMode false

// 3. 查看配置文件
cat .git/config

// 4. 如果配置文件中看到fileMode false表明配置成功
```