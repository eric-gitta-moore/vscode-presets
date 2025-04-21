# vscode-presets

vscode 查看推荐的扩展
```
@recommended 
```

全平台通用导出
- 需要安装 jq
```sh
code --list-extensions | jq -R -n '[inputs] | {recommendations: .}' | jq -S '.' | code -
```

windows 写入剪贴板
```sh
echo xxx | clip
```

macOS 写入剪贴板
```sh
echo xxx | pbcopy
```
