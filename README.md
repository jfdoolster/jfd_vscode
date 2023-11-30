# CURRENT:

windows (powershell)
```bash
%APPDATA%\Code
mv ./User ./.User.bak
git clone git@github.com:jfdoolster/jfd_vscode.git User
```


## OLD:

windows (powershell)
```powershell
# create
cmd /c mklink /h  %APPDATA%\Code\User\settings.json  .\settings.json
cmd /c mklink /j  %APPDATA%\Code\User\snippets       .\snippets\

# delete
Remove-Item -Path %APPDATA%\Code\User\settings.json
Remove-Item -Path %APPDATA%\Code\User\snippets
```

linux
```bash
mkdir -p  $HOME/.config/Code\ -\ OSS/User/snippets
ln -vf ./settings.json  $HOME/.config/Code\ -\ OSS/User/settings.json
ln -vf ./snippets/*     $HOME/.config/Code\ -\ OSS/User/snippets
```
