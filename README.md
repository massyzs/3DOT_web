# Nerfies

This is the repository that contains source code for the [Nerfies website](https://nerfies.github.io).

## 项目概览

- `index.html`：单页网站的主体结构，包含导航、论文摘要、亮点等内容。
- `static/css/`：样式文件，`index.css` 负责自定义外观，其余为 Bulma 等库的编译版本。
- `static/js/index.js`：交互逻辑，目前仅用于插值图片滑块。
- `static/images/` 与 `static/interpolation/`：静态图片资源和插值序列帧。
- `static/videos/`：原始示例中的视频素材；如果不再需要可整目录删除节省空间。

## 如何增删内容

1. **修改文本或模块**：直接编辑 `index.html` 中相应的 `<section>` 块即可。推荐保留 Bulma 的类名以避免额外样式调整。
2. **添加新图文**：将图片放入 `static/images/`，然后在 `index.html` 中引用；如需新样式可在 `static/css/index.css` 追加规则。
3. **删除多余资源**：清理未使用的图片、插值帧或视频时，确保页面中没有残留引用路径。
4. **交互功能**：若要添加新的滑块或按钮，可在 `static/js/index.js` 中扩展，记得同时在 `<head>` 中引入所需库。

本仓库当前已移除所有视频展示段落，如需重新引入，往 `index.html` 添加 `<video>` 或外部嵌入框，并在 `static/videos/` 放置对应文件即可。

If you find Nerfies useful for your work please cite:
```
@article{park2021nerfies
  author    = {Park, Keunhong and Sinha, Utkarsh and Barron, Jonathan T. and Bouaziz, Sofien and Goldman, Dan B and Seitz, Steven M. and Martin-Brualla, Ricardo},
  title     = {Nerfies: Deformable Neural Radiance Fields},
  journal   = {ICCV},
  year      = {2021},
}
```

# Website License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
