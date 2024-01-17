# AlwaysAdminVS
If you're like me and often forget to run VS as admin and proceed to have problems until you feel like an idiot and restart, then this fix is for you

Copy the codeblock below into a .reg file and run it. The reason I don't give you a regfile directly is both so that you can check the contents and avoid annoying antivirus soft.

```
Windows Registry Editor Version 5.00

[HKEY_CURRENT_USER\Software\Microsoft\Windows NT\CurrentVersion\AppCompatFlags\Layers]
"C:\\Program Files\\Microsoft Visual Studio\\2022\\Professional\\Common7\\IDE\\devenv.exe"="RUNASADMIN"
"C:\\Program Files (x86)\\Common Files\\Microsoft Shared\\MSEnv\\VSLauncher.exe"="RUNASADMIN"
```
