# Modern NUDT Slides

基于 Typst 和 Touying 的非官方演示文稿模板，适用于组会、文献汇报和项目展示。

## 快速开始

安装 [Typst](https://typst.app/)，在模板目录中编译示例：

```sh
typst compile main.typ main.pdf
```

首次编译需要联网获取 Touying 和主题依赖。

## 配置与组件

在 `main.typ` 的 `use-theme` 中填写标题、副标题、汇报人、日期和单位。`toc-mode` 控制目录页：`"none"` 不显示目录，`"once"` 只显示总目录，`"full"` 同时显示总目录和每章目录，默认值为 `"full"`。保留 `#toc-slide()` 调用，由该选项统一控制总目录。

`highlight-box` 可突出公式或结论；宽度、高度、圆角、内边距、描边和底色均可覆盖：

```typst
#highlight-box[
  *缩放点积注意力*
  #align(center)[$"Attention"(Q, K, V) = "softmax"(Q K^T / sqrt(d_k)) V$]
]
```

代码片段可使用 `#compact-code("x = y + z")` 排版。更多示例见 `main.typ`。

## 文件

- `main.typ`：演示文稿内容和封面信息。
- `theme.typ`：主题样式与可复用组件。
- `images/`：封面和页眉使用的图片资源。

修改配色、字体或页眉页脚时编辑 `theme.typ`；替换图片时保留文件名，或同步更新 `main.typ` 和主题中的引用。

## 来源与许可

本模板基于 [Touying Simpl NUDT](https://typst.app/universe/package/touying-simpl-nudt) 开发。项目代码采用 [MIT License](LICENSE)。

`images/logo.png` 和 `images/nudt-vi-nudtbg.png` 属于国防科技大学视觉识别资源，不包含在本项目的 MIT 许可中。使用或再分发这些图片时，请遵循学校的品牌与知识产权规范；其他上游内容仍受其各自许可约束。
