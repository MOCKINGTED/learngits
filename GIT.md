### 1. ����
```
// 1.  ��Ŀ����һ��Ŀ¼��
git init
git config --global user.name "TED"
git config --global user.email "lhy19980302@163.com"

// 2. ��Ŀ����һ��Ŀ¼��
git pull

// 3.  ������Կ���ܣ���ȡ�ù�Կ������GITHUB��
ssh-keygen
cat ~/.ssh/id_rsa.pub

//  4. ��¡��Ŀ
git clone git@github(github����ssh�ĵ�ַ)

// 5. ������Ŀ��ַ
cd ��Ŀ
```git
### 2. һ�㲽��
```git
// 1. ���������ļ������ݴ���
git add �ļ���

// 2. �ύ����
git commit . -m "���Ǳ�ע��Ϣ"

// 3. �ϴ����汾��
```

### 2. �Ƚ�
```git

//  1. �ȽϹ������䶯
git diff

//  2. �������Ƚ��ݴ����䶯
git status

// 3. �ݴ�������һ�ΰ汾��Ƚ�
git diff --cached �ļ���

// 4.�ݴ�����ָ����¼�Ƚ�
git log 		# 1. �ҵ�ָ��hashֵ
git diff hashֵ 	# 2. ���������ҵ���hashֵ

// 5. �ݴ��������°汾��Ƚ�
git diff HEAD

// 6. ������ʷ�汾�Ƚ�
git diff hashֵ1 hashֵ2
```

### 3. �����ļ�Ȩ��
```git
// 1. ��ǰ�汾������ļ�Ȩ����Ϣ
git config core.filemode false

// 2. ��ǰ���Ե����а汾������ļ�Ȩ����Ϣ
git config --global core.fileMode false

// 3. �鿴�����ļ�
cat .git/config

// 4. ��������ļ��п���fileMode false�������óɹ�
```