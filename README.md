# 广东大学生校外觅食技巧

写给在外省读书的广东学生的校外觅食指南，用 Markdown 写成，配 Just the Docs 主题发布在 GitHub Pages 上。

## 内容

| 文件 | 内容 |
| --- | --- |
| [index.md](index.md) | 首页 |
| [找店篇.md](找店篇.md) | 待整理 |
| [点菜篇.md](点菜篇.md) | 已整理 |
| [沟通篇.md](沟通篇.md) | 待整理 |
| [观察篇.md](观察篇.md) | 待整理 |

每篇最上面的 `title` 和 `nav_order` 控制左边导航栏里的名字和顺序，改这两个就行。

## 发布到 GitHub Pages

1. 在 GitHub 上新建一个公开仓库，名字建议用 `Meal`（新建时不要勾选 Add a README file）。
2. 在本目录下推送代码：

   ```
   git remote add origin https://github.com/<你的用户名>/Meal.git
   git push -u origin main
   ```

3. 打开仓库的 **Settings → Pages**：
   - Source 选 **Deploy from a branch**
   - Branch 选 **main**，目录选 **/ (root)**
   - 点 **Save**
4. 等一两分钟，网站就出现在 `https://<你的用户名>.github.io/Meal/`。

## 注意事项

- 网站通过 `remote_theme` 直接引用 Just the Docs 主题，不需要在本地安装 Jekyll；本机目前也没有装 Ruby，想本地预览的话需要另外安装。
- 仓库名如果不是 `Meal`，把 [_config.yml](_config.yml) 里的 `baseurl` 改成 `/仓库名`；如果用的是 `<用户名>.github.io` 这种个人主页仓库，`baseurl` 留空字符串。
- 页面之间的链接用了 Jekyll 的 `{% link %}` 写法，改动文件名时记得同步改链接。
