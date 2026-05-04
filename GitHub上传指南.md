# GitHub 上传指南（图文步骤）

不用害怕，跟着做就行，每一步都有说明。

---

## 第一步：安装 Git

1. 打开浏览器，访问：**https://git-scm.com/downloads/win**
2. 下载 Windows 版本，双击安装
3. 安装过程中**一直点「Next」**，用默认设置即可
4. 安装完成后，按 `Win + R`，输入 `cmd`，回车
5. 在黑色窗口中输入 `git --version`，如果显示版本号，说明安装成功

---

## 第二步：注册 GitHub 账号

1. 打开：**https://github.com**
2. 点击右上角「Sign up」
3. 填写邮箱、密码、用户名，完成注册
4. 登录后进入你的个人主页

---

## 第三步：创建仓库

1. 点击右上角 **"+"** → **"New repository"**
2. 填写：
   - **Repository name**：`accounting-app`（或任意名字）
   - **Description**：个人记账应用
   - 选择 **Public**（公开）
   - ⚠️ **不要勾选** "Add a README file"（我们已经有了）
3. 点击绿色按钮 **"Create repository"**
4. 创建后会跳转到一个页面，**记下那个页面显示的仓库地址**，类似：
   ```
   https://github.com/你的用户名/accounting-app.git
   ```

---

## 第四步：上传代码

打开 cmd（Win+R → cmd → 回车），逐条粘贴执行以下命令：

```bash
# 1. 进入项目文件夹
cd "C:\Users\luo'xiang\WorkBuddy\20260504214658\accounting-app"

# 2. 初始化 Git 仓库
git init

# 3. 添加所有文件
git add .

# 4. 提交（引号内的文字可以自己改）
git commit -m "首次提交：记账应用 v1.0"

# 5. 设置分支名为 main
git branch -M main

# 6. 关联你的 GitHub 仓库（把下面地址换成你自己的！）
git remote add origin https://github.com/你的用户名/accounting-app.git

# 7. 推送代码到 GitHub
git push -u origin main
```

执行第 7 条时可能会弹出一个窗口让你登录 GitHub，输入账号密码即可。

---

## 第五步：验证

1. 刷新你的 GitHub 仓库页面
2. 应该能看到 `index.html`、`README.md`、`过程记录.md` 等文件
3. 复制浏览器地址栏的链接，这就是你要交给老师的**仓库链接**

---

## 🔔 提交给老师时

你需要提交：
- ✅ **GitHub 仓库链接**（如 `https://github.com/xxx/accounting-app`）
- ✅ 仓库包含 `index.html`、`README.md`、`过程记录.md` 三个文件

这样就满足作业要求了！
