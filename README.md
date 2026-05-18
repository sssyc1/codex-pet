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

## 使用方式

1. 选择一个 pet 文件夹，例如 `pets/lili-squirrel`。
2. 将整个 pet 文件夹复制到 `~/.codex/pets/<pet-name>`。
   - Windows 对应路径通常是 `%USERPROFILE%\.codex\pets\<pet-name>`。
   - macOS / Linux 对应路径通常是 `~/.codex/pets/<pet-name>`。
3. 打开 Codex 设置，在宠物选项中选择对应 pet。

## License

本仓库采用 `CC BY-NC-ND 4.0` 许可证。完整许可证说明见 [LICENSE](LICENSE)。
