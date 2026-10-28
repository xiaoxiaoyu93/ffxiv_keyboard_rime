# FFXIV Keyboard for Rime

一个适用于 Rime / 小狼毫 Weasel 的《魔光键影》词库方案。

## 文件

- `ffxiv_keyboard.schema.yaml`：Rime 输入方案
- `ffxiv_keyboard_dict.dict.yaml`：词库
- `default.custom.example.yaml`：加入方案列表的配置示例

## 安装

1. 把 `ffxiv_keyboard.schema.yaml` 和 `ffxiv_keyboard_dict.dict.yaml` 复制到 Rime 用户目录。
2. Windows 小狼毫用户目录通常是：

   ```text
   %APPDATA%\Rime
   ```

3. 编辑用户目录下的 `default.custom.yaml`，在 `patch.schema_list` 中加入：

   ```yaml
   patch:
     schema_list:
       - {schema: ffxiv_keyboard}
   ```

4. 重新部署 Rime。
5. 在小狼毫方案菜单中选择「魔光键影」。

`default.custom.example.yaml` 只提供参考。不要直接覆盖自己的 `default.custom.yaml`，否则可能丢失你原来的方案设置。

## 使用

切换方案后，可以用完整拼音或首字母简拼输入词库内容。

## 许可说明

- Rime 配置文件的许可见 `LICENSE`。
- 词库内容来自《魔光键影词库》及游戏相关文本，仅供 Rime 输入法个人学习与使用。游戏文本和词库原始版权归原权利方所有。