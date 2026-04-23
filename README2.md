
# 🚀 Git + GitHub 标准工作流（SSH版）

## 🧭 一、创建新项目并上传到 GitHub

### 1️⃣ 在 GitHub 创建仓库

* 登录 GitHub
* 点击 `New repository`
* **不要勾选 README（重要）**

---

### 2️⃣ 本地创建项目
直接新建文件夹也行，然后右键 open git bash here
```bash
先 git remote -v
再 git remote set-url origin https://github.com/wslj19951226-oss/neuroscience-test.git #（New repository的地址）

---

### 3️⃣ 添加文件

```bash
echo "# my project" > README.md
```

或直接把你的代码放进这个文件夹

---

### 4️⃣ 添加并提交

```bash
git add .
git commit -m "initial commit"
```

---

### 5️⃣ 设置主分支为 main

```bash
git branch -M main
```

---

### 6️⃣ 连接 GitHub（SSH）

```bash
git remote add origin git@github.com:你的用户名/仓库名.git
```
如 $ git remote set-url origin git@github.com:wslj19951226-oss/neuroscience-test.git

---

### 7️⃣ 首次推送

```bash
git push -u origin main
```

---

## 🔄 二、日常更新代码（最常用）

### 每次修改代码后：

```bash
git add .
git commit -m "update: 描述你的修改"
git push
```

---

## 🔽 三、从 GitHub 拉取更新

```bash
git pull
```

---

## 🌿 四、分支（进阶但推荐）

### 创建新分支

```bash
git checkout -b new-feature
```

### 切换分支

```bash
git checkout main
```

---

## 🔧 五、常见问题解决

### ❌ push 被拒绝

```bash
git pull origin main --rebase
git push
```

---

### ❌ remote 已存在

```bash
git remote set-url origin git@github.com:你的用户名/仓库名.git
```

---

### ❌ 没有 main 分支

```bash
git branch -M main
```

---

## ⚡ 六、推荐习惯（非常重要）

* 永远使用 **SSH（[git@github.com](mailto:git@github.com)）**
* GitHub 创建仓库时不要初始化 README
* 每次修改都写清楚 commit message
* 小步提交，不要一次改很多

---

## 🧠 一句话总结

> 写代码 → add → commit → push

---
