# Oh My Posh Theme

## 创建 `PowerShell` 描述文件

```shell
New-Item -Path $PROFILE -Type File -Force
```
> [!WARNING]
> 
> PowerShell 也可能阻止运行本地脚本
> ```shell
> Set-ExecutionPolicy RemoteSigned
> ```
## 修改描述文件

```shell
notepad $PROFILE 
```

粘贴以下内容

```shell
oh-my-posh init pwsh --config 'https://raw.gitmirror.com/cuiqg/settings/main/ohmyposh/theme.opm.json' | Invoke-Expression
```

## 使配置生效

```shell
. $PROFILE
```
