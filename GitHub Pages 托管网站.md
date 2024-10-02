使用 GitHub Pages 托管网站可以轻松将静态网站托管在 GitHub 仓库中。以下是步骤指南：

### 步骤 1: 创建 GitHub 仓库
1. 登录 GitHub。
2. 点击右上角的 `+` 号，选择 `New repository`。
3. 在 `Repository name` 中输入你想要的仓库名称（例如：`username.github.io`，其中 `username` 是你的 GitHub 用户名）。
4. 选择 `Public`。
5. 点击 `Create repository`。

### 步骤 2: 设置网站文件
1. 本地创建一个文件夹，存放你的静态网站文件。
2. 网站的主页面文件通常命名为 `index.html`。
3. 可以创建简单的 HTML 文件（例如：`index.html`），或者将已有的静态网站文件放入该文件夹中。

#### 例如：`index.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My GitHub Page</title>
</head>
<body>
    <h1>Hello, welcome to my GitHub Pages site!</h1>
</body>
</html>
```

### 步骤 3: 上传代码到 GitHub
1. 打开终端或命令行，进入你的网站文件所在的目录。
2. 初始化 git 仓库，并将文件上传到 GitHub：

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/username.github.io.git
git push -u origin main
```

> 将 `username` 替换为你的 GitHub 用户名。

### 步骤 4: 启用 GitHub Pages
1. 进入你的仓库页面，在顶部菜单点击 `Settings`。
2. 左侧菜单选择 `Pages`。
3. 在 `Source` 部分，选择 `main branch`（或你网站文件所在的分支）。
4. 点击 `Save`。

GitHub 会自动生成并托管你的网站，地址为 `https://username.github.io`。

### 可选步骤：自定义域名
如果你有自定义域名，GitHub Pages 允许你将其绑定到你的仓库。你可以通过在仓库的 `Settings` 页面下的 `Pages` 部分，配置 `Custom domain` 来实现。

### 使用 Jekyll (可选)
如果你想用 Jekyll 来构建静态网站，可以按照以下步骤：
1. 安装 [Jekyll](https://jekyllrb.com/)。
2. 创建一个 Jekyll 站点：
    ```bash
    jekyll new my-website
    cd my-website
    ```
3. 按照上述步骤上传并部署到 GitHub Pages。

这就是使用 GitHub Pages 托管网站的基本流程。