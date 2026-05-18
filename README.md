# Codex Pets

这个仓库用于集中发布多个自制 Codex pet。每个 pet 都是一个独立文件夹，可以单独复制到本机 Codex 的 pets 目录中使用。

## Pets 目录结构

```text
codex-pet/
|-- README.md
|-- LICENSE
|-- pets/
|   |-- lili-squirrel/
|   |   |-- pet.json
|   |   `-- spritesheet.webp
|   `-- trumpy/
|       |-- pet.json
|       `-- spritesheet.webp
```

新增 pet 时，请放在 `pets/<pet-name>/` 目录下，并至少包含：

- `pet.json`
- `spritesheet.webp`

`pet.json` 中的 `spritesheetPath` 字段应指向同目录下的 `spritesheet.webp`。不要写成本机绝对路径，例如 `C:\...`、`D:\...`、`/Users/...` 或 `/home/...`。

## Windows 安装方式

在 PowerShell 中从仓库根目录运行：

```powershell
New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\pets"
Copy-Item -Recurse ".\pets\<pet-name>" "$env:USERPROFILE\.codex\pets\"
```

例如：

```powershell
Copy-Item -Recurse ".\pets\lili-squirrel" "$env:USERPROFILE\.codex\pets\"
```

## macOS / Linux 安装方式

在终端中从仓库根目录运行：

```bash
mkdir -p ~/.codex/pets
cp -R ./pets/<pet-name> ~/.codex/pets/
```

例如：

```bash
cp -R ./pets/lili-squirrel ~/.codex/pets/
```

## 使用方式

1. 选择一个 pet 文件夹，例如 `pets/lili-squirrel`。
2. 将整个 pet 文件夹复制到 `~/.codex/pets/<pet-name>`。
   - Windows 对应路径通常是 `%USERPROFILE%\.codex\pets\<pet-name>`。
   - macOS / Linux 对应路径通常是 `~/.codex/pets/<pet-name>`。
3. 打开 Codex 设置，在宠物选项中选择对应 pet。

## License

本仓库采用 `CC BY-NC-ND 4.0` 许可证。原作者 / 仓库链接：[sssyc1/codex-pet](https://github.com/sssyc1/codex-pet)。

允许：

- 个人非商业使用。
- 分享原始、未修改的文件。
- 本地私下修改，但不得发布、分发或公开提供修改后的版本。
- 出现在非商业视频、教程、博客、截图、演示中。

必须：

- 署名原作者，并附上本仓库链接。

禁止：

- 商业使用。
- 销售、打包售卖、商业产品集成。
- 发布修改版、换色版、二创版、衍生宠物包，除非获得作者明确许可。

完整许可证说明见 [LICENSE](LICENSE)。
