# Modern NUDT Touying 汇报模板

基于 Typst 和 Touying 的非官方演示文稿模板，适合组会汇报、文献分享和项目汇报。

## 使用

需要安装 [Typst](https://typst.app/) 并联网获取 Touying 及主题依赖。进入本目录后编译：

```sh
typst compile main.typ main.pdf
```

## 修改内容

- 在 `main.typ` 开头修改标题、副标题、汇报人、日期和单位。
- 替换示例章节与内容；可参考示例中的标题、列表、表格、公式和代码写法。
- 在 `theme.typ` 中调整配色、字体、页眉页脚等主题样式。
- 图片放在 `images/` 下，并在 `main.typ` 中使用 `#image("images/文件名.png")` 引用。

请保留 `theme.typ` 与 `images/` 目录结构，以便封面和主题组件正常显示。

## 来源与版权

本模板基于 [Touying Simpl NUDT](https://typst.app/universe/package/touying-simpl-nudt) 开发。代码采用 [MIT License](LICENSE)。

`images/logo.png` 和 `images/nudt-vi-nudtbg.png` 属于国防科技大学视觉识别资源，不包含在本项目的 MIT 许可中。使用或再分发这些图片时，请遵循学校的品牌与知识产权规范；其他上游内容仍受其各自许可约束。
