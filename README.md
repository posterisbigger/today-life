# 今日生活网站

一个简单的单页面网站，使用HTML+CSS+原生JavaScript开发，所有数据使用浏览器localStorage存储。

## 功能说明

1. **登录/注册功能**
   - 首次使用时自动注册，将用户名和密码保存到localStorage
   - 非首次使用时进行登录验证
   - 登录失败次数达到3次时显示励志提示
   - 登录成功后进入主界面

2. **核心按钮功能**
   - 第1次点击：提示"今天会是美好的一天"
   - 第2次及之后点击：提示"请不要把时间浪费在这里，请开始你精彩的一天吧"

## 如何让任何人访问您的网站

以下是使用GitHub Pages部署网站的详细步骤：

### 步骤1：在GitHub上创建新仓库

1. 打开浏览器，登录您的GitHub账号（使用提供的账号：posterisbigger@163.com）
2. 点击右上角的"+"号，选择"New repository"
3. 仓库名称可以设置为"today-life"或任何您喜欢的名称
4. 选择"Public"（公开）仓库
5. 不要勾选"Initialize this repository with a README"（因为我们已经有README文件了）
6. 点击"Create repository"

### 步骤2：将本地仓库推送到GitHub

在本地仓库目录下（即包含index.html的文件夹），打开命令行工具，执行以下命令：

```bash
# 添加远程仓库地址（将your-username替换为您的GitHub用户名，your-repo-name替换为您创建的仓库名称）
git remote add origin https://github.com/posterisbigger/today-life.git

# 推送本地仓库到GitHub
git push -u origin master
```

### 步骤3：启用GitHub Pages

1. 在GitHub仓库页面，点击"Settings"选项卡
2. 向下滚动到"GitHub Pages"部分
3. 在"Source"下拉菜单中，选择"master branch"
4. 点击"Save"按钮
5. 等待几分钟，刷新页面
6. 在"GitHub Pages"部分，您将看到一个URL，例如：https://your-username.github.io/your-repo-name/

### 步骤4：访问您的网站

现在，任何人都可以通过上述URL访问您的网站了！

## 本地运行

如果您想在本地运行和测试网站，只需将index.html文件用浏览器打开即可。

## 注意事项

1. 网站使用浏览器localStorage存储数据，每个访问者的数据都存储在他们自己的浏览器中，不会相互影响
2. GitHub Pages提供的是免费的静态网站托管服务，非常适合个人网站
3. 部署完成后，每次修改代码并推送到GitHub，网站会自动更新

## 技术实现

- 纯HTML+CSS+原生JavaScript
- 使用localStorage存储用户信息和点击次数
- 浏览器原生alert弹窗
- 温馨励志的暖黄色/浅橙色系设计风格