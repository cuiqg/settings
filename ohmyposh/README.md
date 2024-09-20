# Oh My Posh Theme

## 使用

```powershell
notepad $PROFILE
```

> [!NOTE]
> When the above command gives an error, make sure to create the profile first and add the oh-my-posh init above.
> ```powershell
> New-Item -Path $PROFILE -Type File -Force
> ```
> In this scenario, it can also be that PowerShell blocks running local scripts. To solve that, set PowerShell to only require remote scripts to be
> signed using Set-ExecutionPolicy RemoteSigned, or sign the profile.
>

粘贴以下内容

```powershell
oh-my-posh init pwsh --config "https://raw.gitmirror.com/cuiqg/settings/refs/heads/main/ohmyposh/theme.omp.json" | Invoke-Expression
```
