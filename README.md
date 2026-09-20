# 广东大学生校外觅食技巧

写给在外省读书的广东学生的校外觅食指南，用 Markdown 写成，配 Just the Docs 主题发布在 GitHub Pages 上。

- 仓库：<https://github.com/FiddieMath/CantoneseEating>
- 网站（启用 Pages 后）：<https://fiddiemath.github.io/CantoneseEating/>

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

1. 推送代码（如果还没配 remote、也没推过）：

   ```
   git remote add origin https://github.com/FiddieMath/CantoneseEating.git
   git push -u origin main
   ```

2. 打开 <https://github.com/FiddieMath/CantoneseEating/settings/pages>：
   - Source 选 **Deploy from a branch**
   - Branch 选 **main**，目录选 **/ (root)**
   - 点 **Save**

3. 等一两分钟，网站出现在 <https://fiddiemath.github.io/CantoneseEating/>。

## 以后更新内容

改完 Markdown 之后：

```
git add -A
git commit -m "更新点菜篇"
git push
```

推上去一两分钟，网站自动更新。

## 注意事项

- `_config.yml` 里的 `baseurl` 已经按仓库名 `CantoneseEating` 设置好。如果哪天改了仓库名，记得同步改这里。
- 网站通过 `remote_theme` 引用 Just the Docs 主题，本地不需要安装 Ruby；想在本地预览才需要装 Jekyll。
- 页面之间的链接用了 Jekyll 的 `{% link %}` 写法，改动文件名时记得同步改链接。
