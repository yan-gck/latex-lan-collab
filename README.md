# LaTeX 局域网协作

用桌面版 VS Code 在同一局域网共同编辑 LaTeX 工程。主持人保存工程文件、编译和发布 PDF，参与者可同时编辑同一个章节，也可分别写不同文件。

## 安装

1. 打开[最新发行版](https://github.com/yan-gck/latex-lan-collab/releases/latest)，在 **Assets** 中下载以 `.vsix` 结尾的文件。
2. 在 VS Code 1.95 或更新版本按 `Ctrl+Shift+P`（macOS 为 `⌘⇧P`），执行 **Extensions: Install from VSIX…**，选择刚下载的文件。
3. 主持人打开工程文件夹，按 `F1` 执行 **LaTeX 局域网协作：创建协作会话**，将邀请链接发给队友。
4. 参与者执行 **LaTeX 局域网协作：加入协作会话**，粘贴链接并打开章节。参与者按保存快捷键后会等待主机确认落盘。

## 写作与预览

- 选中 LaTeX 文本后可用 `Ctrl+B`、`Ctrl+I`、`Ctrl+U` 加粗、设为斜体或添加下划线。在 macOS 上使用 `⌘`。
- 主持人可通过 LaTeX Workshop 编译，参与者无需安装 TeX。双方通过 **发布或查看 PDF** 打开预览。
- 使用 `-synctex=1` 编译后，协作 PDF 中双击可跳到对应源码行。打开协作预览后，在共享源码中双击词语即可定位到 PDF，也可使用 `Alt+Shift+J`。
