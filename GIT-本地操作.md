### 1. ����
```
1.  ��Ŀ����һ��Ŀ¼��
git init
git config --global user.name "TED"
git config --global user.email "lhy19980302@163.com"

2. ��Ŀ����һ��Ŀ¼��
git pull

3.  ������Կ���ܣ���ȡ�ù�Կ������GITHUB��
ssh-keygen
cat ~/.ssh/id_rsa.pub

4. ��¡��Ŀ
git clone git@github(github����ssh�ĵ�ַ)

5. ������Ŀ��ַ
cd ��Ŀ
```

### 2. һ�㲽��
```git
1. ���������ļ������ݴ���
git add �ļ���

2. �ύ����
git commit . -m "���Ǳ�ע��Ϣ"

3. �ϴ����汾��
```

### 2. �Ƚ�
```git

�ȽϹ������䶯
git diff

�������Ƚ��ݴ����䶯
git status

1. �ݴ�������һ�ΰ汾��Ƚ�
git diff --cached �ļ���

1.�ݴ�����ָ����¼�Ƚ�
git log 		# 1. �ҵ�ָ��hashֵ
git diff hashֵ 	# 2. ���������ҵ���hashֵ

�ݴ��������°汾��Ƚ�
git diff HEAD

������ʷ�汾�Ƚ�
git diff hashֵ1 hashֵ2
```

### 3. �����ļ�Ȩ��
```git
1. ��ǰ�汾������ļ�Ȩ����Ϣ
git config core.filemode false

2. ��ǰ���Ե����а汾������ļ�Ȩ����Ϣ
git config --global core.fileMode false

3. �鿴�����ļ�
cat .git/config

4. ��������ļ��п���fileMode false�������óɹ�
```

### 4.1 ��git�����ļ�
- `.gitignore`�ļ�����Ҫ�ŵ��汾������
1. �����Զ����ɵ��ļ�
2. ���Ա������ɵ��м��ļ���һϵ���Զ����ɵ��ļ�
3. ���Դ���������Ϣ�������ļ��������ſ���������ļ�

```
1. ����.gitignore�ļ�
touch .gitignore
2. ����Ҫ���ӵ��ļ������Ƽ��룬ÿ��һ��
.DS_store
.idea


```
### 4.2 ��git��ӻ��������ļ�
```
1. ʹ��git�������
git check-ignore -v .DS_store

1. ʹ��ǿ�����
```

## 5 ��֧����
- ����ʹ��`master`��֧��������`develop`��֧, �޸�bug��`test`��֧

### 5.1 �鿴��֧
```
�鿴���ط�֧
git branch

�鿴���غ�Զ�̷�֧
git branch -a
```

### 5.2 �½���֧
```
����Զ�̷�֧
git checkout master

1. �½����ط�֧
git checkout -b ��֧��
2. ָ��Զ�̷�֧��
git push --set-upstream origin ��֧��
```

### 5.3 �ϲ���֧
```
����֧�ϲ���master��
git merge test
```

### 5.4 ɾ����֧
```
��ͨɾ��
git branch -d ��֧��

ǿ��ɾ��
git branch -D ��֧��
```