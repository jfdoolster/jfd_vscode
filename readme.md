
windows (powershell)
```bash
cmd /c mklink /j $HOME\AppData\Roaming\Code\User\snippets .\snippets\
cmd /c mklink /h $HOME\AppData\Roaming\Code\User\settings.json .\settings.json
```

linux
```bash
ln -s ./snippets $HOME/.config/Code\ OSS/User/snippets
ln -h ./settings.json $HOME/.config/Code\ OSS/User/settings.json
```