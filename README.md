# 代码编辑

MyPaste extension `com.mypaste.code-edit` (version `3.7.2`).

在本地编辑代码或纯文本：行号、语法高亮、语言识别与格式化都随包提供，所有语言的格式化都在扩展内完成，不依赖本机安装 gofmt、rustfmt、Python、Prettier 或其它工具；本机有 Node 时，CSS、YAML、JavaScript 与 TypeScript 会改用包内 Prettier 或内置脚本，排版更完整，没有也照常可用；顶部是可编辑标题的文档头，「语言」与「格式化」两个下拉按当前语言列出内置格式化与 SQL 压缩；高亮完全本地，不依赖其它能力包。可另存为新的历史条目或复制到剪贴板，原条目保持不变，不联网、不读取其它条目。

This repository is an independent copy extracted from the former `mypaste-code-extensions` monorepo at commit `2af6675ab1473c9e38146ea0b6da68256a293440`. It contains only this extension's tracked source files. The published `.mypaste-plugin` archives and marketplace index live in [`mypaste-extensions-catalog`](https://github.com/mypaste/mypaste-extensions-catalog).

The manifest speaks MyPaste plugin protocol v3. Installation, capability mediation, and content-digest verification are performed by the MyPaste desktop host.

## Files

- `mypaste.plugin.json`: package identity and capability declaration.
- `run.sh`, `src/`, `panel.html`, or `run`: package implementation.

## Build

```bash
bun install
bun run build
```

The generated `preview.html` is intentionally ignored; edit `src/preview.html` and `src/main.ts` instead.

## License

MIT. See [LICENSE](LICENSE).
