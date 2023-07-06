windows (powershell)
```powershell
# create
cmd /c mklink /j $HOME\AppData\Roaming\Code\User\snippets      .\snippets\
cmd /c mklink /h $HOME\AppData\Roaming\Code\User\settings.json .\settings.json

# delete
Remove-Item -Path $HOME\AppData\Roaming\Code\User\settings.json
Remove-Item -Path $HOME\AppData\Roaming\Code\User\snippets
```

linux
```bash
mkdir -p $HOME/.config/Code\ -\ OSS/User/snippets
ln -vf ./snippets/*    $HOME/.config/Code\ -\ OSS/User/snippets
ln -vf ./settings.json $HOME/.config/Code\ -\ OSS/User/settings.json
```
