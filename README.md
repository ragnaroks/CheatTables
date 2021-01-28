# CheatTables
Cheat Engine 作弊表

### CT表命名格式
`{发行平台}-[{可执行文件名}]-{处理器架构}-{可执行文件SHA1}.ct`

例子：
- steam-[ExampleGame-Win64-Shipping]-amd64-3955A4217A4E41DF0C361C11CA27AF955DBB0130.ct
- uplay-[Future Soldier DX9]-x86-120C4B89B8B8F3D5D65CE61DDB63DC446C861F64.ct
- multi-[SomeGame]-amd64-multi.ct

**可执行文件名**字段必须与原始文件夹保持完全一致

**发行平台**字段可选项：`indie`、`steam`、`uplay/ubc`、`epic`、`gog`、`origin/eaapp/eadm`，当表单适用于多个平台时可用`multi`

**处理器架构**字段可选项：`x86`、`amd64/x64`、`aarch64`

**可执行文件SHA1**字段大小写任意，如果表单适用于多个版本的游戏可用`multi`

### 路径结构
```plain
|- Year
|  |- GameName
|  |  |- README.md
|  |  |- cheat-table.ct
|
├─ 2009
│  ├─ Alien Shooter
│  │  |- README.md
│  │  |- steam-[AlienShooter]-x86-63CBC62239C8C0A4272B852AC696817D6216CAFC.ct
│  │      
│  ├─ Alien Shooter 2：Reloaded
│  |  |- README.md
│  |  |- steam-[AlienShooter]-x86-532B783C83AE67F40BAF409B340A0993E37DEB23.ct
```

### 贡献指南
> 不接受任何多人游戏和网络游戏的表单，但同时拥有离线单机模式和联网对战模式的游戏可提交，且该表单只能有离线单机部分的功能

在相应文件夹内创建如上命名格式的表单，并在文件夹内的 README.md 中以如下形式附加说明。
```markdown
### uplay-[Future Soldier DX9]-x86-120C4B89B8B8F3D5D65CE61DDB63DC446C861F64
- 只适用于 DX9 版本
- 无限子弹和无限弹匣不要同时开启
......
```

如果还没有相应文件夹或文件夹内不存在 README.md 文件，可自行创建

对表单质量没有要求，即使此表单可能造成游戏崩溃、反作弊侦测、系统不稳定等，由使用者自行承担后果，但不允许表单有恶意代码，特别是 lua 代码

如果游戏有多个发行平台，以最早发行时间为准，比如 GTAV 于 2013 年发行于 PS3 平台，2015 年发行于 PC 平台（steam、rockstar），则相关表单应位于 2013 文件夹中；如果表单是第 1 次提交，可基于制作时对应平台的发布时间，比如为 GTAV 制作的表单适用于 steam 平台，则相关表单可位于 2015 文件夹中，将在后续移动于 2013 文件夹中；如果游戏有多个独立版本，比如 Call of Duty：Modern War 及其重置版，应视为两个不同游戏分别放置在对应年份的文件夹中

游戏名字文件夹中如果出现`:`（英文冒号）一律以`：`（中文冒号）替代以兼容文件系统

不允许对他人表单直接进行 PR 修改，建议以 Issue 的形式沟通处理

### 提交消息
提交的 title（即第 1 行） 为游戏名，提交的 message（即第 3 行及更多） 为**动作**及**脚本名称**，可附加说明，第 2 行固定为换行

建议使用 `git commit -m title -m message1 -m message2` 的方式提交

```git-commit
Tom Clancy's Ghost Recon：Future Soldier

更新 uplay-[Future Soldier DX9]-x86-120C4B89B8B8F3D5D65CE61DDB63DC446C861F64，修复了一些错误
```

### 其它注意事项
除非表单作者已提前明确允许，任何第三方分发或基于商业目的的使用本仓库任何表单，均需联系表单作者

本仓库默认面向中文用户，需确保能正确理解中文的意思，表单如果部分或全部功能失效，请使用真诚的文本在 Issue 中提出，因为作者们都是无偿贡献，[此为反面典型](https://bbs.3dmgame.com/forum.php?mod=viewthread&tid=6097527)