# CheatTables
Cheat Engine 作弊表

### CT表命名格式
{发行平台}-[{可执行文件名}]-{架构}-{可执行文件SHA1}-{作者}

- `steam-[ExampleGame-Win64-Shipping]-amd64-3955A4217A4E41DF0C361C11CA27AF955DBB0130-ragnaroks`
- `uplay-[Future Soldier DX9]-x86-120C4B89B8B8F3D5D65CE61DDB63DC446C861F64-ragnaroks`

**发行平台**字段可选项：`'indie','steam','uplay','epic','gog'`

**架构**字段可选项：`'x86','amd64/x64','aarch64'`

如果脚本来自别处，除非已明确允许转载，否则需得到原始作者许可，并在相应 README.md 文件中注明原始链接或可查出处。

脚本文件名出现 `'` 字符时使用 `‘` 替换以避免出现混淆。

### 贡献指南
在相应文件夹内创建如上命名格式的表单，并在文件夹内的 README.md 中以如下形式附加说明。
```plain
### uplay-[Future Soldier DX9]-x86-120C4B89B8B8F3D5D65CE61DDB63DC446C861F64-ragnaroks
只适用于 DX9 版本。
无限子弹和无限弹匣不要同时开启。
...
```

如果还没有相应文件夹或文件夹内不存在 README.md 文件，可自行创建。

如果脚本支持多个可执行文件，可使用 `uplay-[Future Soldier DX9]-x86-multi` 格式表达，但更推荐将表单复制多份并改名相应可执行文件哈希。

对表单质量没有要求，即使此表单可能造成游戏崩溃、反作弊侦测、系统不稳定等，需要使用者自行承担后果。

默认情况下，不允许对他人表单进行修改，建议以 Issue 的形式沟通处理。

### 注意事项
**不接受任何多人游戏的表单。**

除非表单作者已提前明确允许，第三方分发或基于商业目的的使用需联系作者。

部分早期表单格式错误，但不确定是否仍然有效，如果发现已失效可在 Issue 中指出。

表单如果部分或全部功能在游戏更新后失效，请使用诚恳的语气在 Issue 中提出，因为作者都是无偿贡献；另外本仓库是中文使用环境，需确保能正确理解中文的意思；[此为反面典型](https://bbs.3dmgame.com/forum.php?mod=viewthread&tid=6097527)。