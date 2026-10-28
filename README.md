# FFXIV Keyboard for Rime

一个适用于 Rime / 小狼毫 Weasel 的《魔光键影》词库方案。

## 下载小狼毫

- 官方下载页：<https://rime.im/download/>
- GitHub Releases：<https://github.com/rime/weasel/releases>

## 文件

- `ffxiv_keyboard.schema.yaml`：Rime 输入方案
- `ffxiv_keyboard_table.dict.yaml`：表格式词库，包含全拼紧凑码和首字母简拼码

## 安装

1. 安装小狼毫 Weasel。
2. 把 `ffxiv_keyboard.schema.yaml` 和 `ffxiv_keyboard_table.dict.yaml` 复制到 Rime 用户目录。
3. Windows 小狼毫用户目录通常是：

   ```text
   %APPDATA%\Rime
   ```

4. 编辑用户目录下的 `default.custom.yaml`，在 `patch.schema_list` 中加入：

   ```yaml
   patch:
     schema_list:
       - {schema: ffxiv_keyboard}
   ```

5. 重新部署 Rime。
6. 在小狼毫方案菜单中选择「魔光键影」。

## 游戏内建议配置

如果在 FFXIV 游戏内看不到正在输入的编码，建议编辑小狼毫的用户配置：

```text
%APPDATA%\Rime\weasel.custom.yaml
```

加入：

```yaml
patch:
  app_options/ffxiv_dx11.exe:
    inline_preedit: true
```

然后重新部署小狼毫。若游戏进程名不同，请把 `ffxiv_dx11.exe` 替换为实际的 `.exe` 名称。

## 使用

切换方案后，可以输入：

- 全拼紧凑码，例如 `shenluo`
- 首字母简拼，例如 `sl`

因为使用 `table_translator`，输入部分编码时也会出现候选。

## 许可说明

- Rime 配置文件的许可见 `LICENSE`。
- 词库内容来自《魔光键影词库》及游戏相关文本，仅供 Rime 输入法个人学习与使用。游戏文本和词库原始版权归原权利方所有。