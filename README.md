# vscode-presets

全平台通用导出
- 需要安装 jq
```sh
code --list-extensions | jq -R '[inputs] | {recommendations: .}' | jq -S '.'
```

windows 写入剪贴板
```sh
echo xxx | clip
```

macOS 写入剪贴板
```sh
echo xxx | pbcopy
```
