### Install Extensions

Make sure the `code`/`cursor` command is installed in PATH
- `Ctrl/Cmd + Shift + P`
- `Shell Command: Install 'code' command in PATH`

#### VSCode
```sh
cat extensions.json | jq -r '.recommendations[]' | xargs -I {} code --install-extension {}
```

#### Cursor
```sh
cat extensions.json | jq -r '.recommendations[]' | xargs -I {} cursor --install-extension {}
```
