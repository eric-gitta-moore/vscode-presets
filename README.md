# vscode-presets

windows 导出
```pwsh
echo "{ ""recommendations"": $(code --list-extensions | ConvertTo-Json) }" | jq -S .
```

unix 导出
```bash
code --list-extensions | jq -R '[inputs] | {recommendations: .}' | jq -S '.'
```
