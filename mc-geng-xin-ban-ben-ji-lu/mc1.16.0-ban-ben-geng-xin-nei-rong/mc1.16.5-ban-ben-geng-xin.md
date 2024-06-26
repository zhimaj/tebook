# MC1.16.5版本更新



> ## **【更新】1.16.5版本补丁更新公告：BC1.16.5**
>
> 更新补丁版本：1.16.5
>
> 更新时间：2024-12-12
>
> 更新内容：

### 新内容

#### 命令格式

`/`[`gametest`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/gametest)

* 用于测试GameTest功能。

#### 常规

[环境音效](https://minecraft.fandom.com/zh/wiki/%E7%8E%AF%E5%A2%83%E9%9F%B3%E6%95%88)

* 为[下界](https://minecraft.fandom.com/zh/wiki/%E4%B8%8B%E7%95%8C)加入了新的环境音效。[\[4\]](https://minecraft.fandom.com/zh/wiki/%E5%9F%BA%E5%B2%A9%E7%89%881.16.210#cite\_note-4)
  * 不同的下界生物群系会播放不同的环境音效。

[实验性玩法](https://minecraft.fandom.com/zh/wiki/%E5%AE%9E%E9%AA%8C%E6%80%A7%E7%8E%A9%E6%B3%95)

* 加入了“启用游戏测试框架”子选项。

[选项](https://minecraft.fandom.com/zh/wiki/%E9%80%89%E9%A1%B9)

* 在声音设置里加入了文本转语音选项。

#### 技术性

GameTest框架

* 一个基于将测试代码与测试结构配对的服务端测试的自动工具。
* 在主机平台上不可用。
* 仅开启[实验性玩法](https://minecraft.fandom.com/zh/wiki/%E5%AE%9E%E9%AA%8C%E6%80%A7%E7%8E%A9%E6%B3%95)（启用游戏测试框架子选项）后可用。

### 更改

#### 方块

[红石粉](https://minecraft.fandom.com/zh/wiki/%E7%BA%A2%E7%9F%B3%E7%B2%89)

* 英文名称重命名为“Redstone Dust”，以与[Java版](https://minecraft.fandom.com/zh/wiki/Java%E7%89%88)统一。

#### 命令格式

`/`[`camerashake`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/camerashake)

* 加入了停止动作的命令。

`/`[`clone`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/clone)、`/`[`fill`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/fill)、`/`[`setblock`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/setblock)

* 加入了新的命令选项，用于选择放置方块时方块的初始状态。

`/`[`mixer`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/mixer)

* 将此命令完全移除。

`/`[`structure`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/structure)

* 现在使用命令`/`[`structure`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/structure) `delete`可以删除已保存结构列表。

#### 常规

辅助功能

* 更改了下列选项名称：
  * “启用聊天文本转语音”更改为“聊天文本转语音”。
  * “启用设备设置启用文本转语音”更改为“设备设置文本转语音”。
  * “启用UI界面阅读器”更改为“UI界面阅读器”。

[选项](https://minecraft.fandom.com/zh/wiki/%E9%80%89%E9%A1%B9)

* 由于Mixer流媒体服务不再可用，游戏将广播选项完全移除。

[控制](https://minecraft.fandom.com/zh/wiki/%E6%8E%A7%E5%88%B6)

* 现在可以通过按下F11快捷键切换至全屏显示模式。

[加载提示](https://minecraft.fandom.com/zh/wiki/%E5%8A%A0%E8%BD%BD%E6%8F%90%E7%A4%BA)

* 加入了一条新的加载提示：
  * “在 iOS、Android 或 FireOS 上游玩？快去市场获取免费的《我的世界》原创音乐包，享受完整的《我的世界》体验吧。”

地图制作和[附加包](https://minecraft.fandom.com/zh/wiki/%E9%99%84%E5%8A%A0%E5%8C%85)

* 在资源包模板中加入了“fogs”文件夹。
* 加入了Fog文档。
* 为方块事件响应`decrement_stack`加入了`ignore_game_mode`布尔参数，默认设置为false。因此`decrement_stack`不再会在创造模式下减少默认物品堆叠。
* 将`RideableComponent`中的属性`rotate_rider_by`更改为支持自定义生物的功能。
* `SetBlock`和`SetBlockAtPos`事件现在支持方块的自定义状态。
* 1.16.2以及之前版本创建的附着物都不会为第一人称下持有它的玩家渲染。1.16.2版本之后创建的除盔甲以外的附着物都可在第一人称下被渲染。

#### 技术性

组件变量

* `main_hand` - 一个可选对象，用于储存玩家右手的`first_person`和`third_person`可选切换数据。
* `off_hand` - 一个可选对象，用于储存玩家左手的`first_person`和`third_person`可选切换数据。
* `first_person` - 一个可选对象，用于储存`position`、`rotation`和`scale`3个向量，以构建第一人称矩阵。
* `third_person` - 一个可选对象，用于储存`position`、`rotation`和`scale`3个向量，以构建第三人称矩阵。

渲染偏移组件

* 如剑或镐等简单物品可以对其应用可选的偏移量以改变其渲染方式。
  * 注意：该组件不应该应用到附加物品中。

### 修复

原版趋同

* 玩家现在可以在下界听到环境音效了。（[MCPE-74756](https://bugs.mojang.com/browse/MCPE-74756)）
  * 手机玩家需要通过商店更新Minecraft原版音乐包才能听到这些新的声音。
* 现在在暖水海洋生物群系中使用骨粉只会生成海草、珊瑚和珊瑚扇。（[MCPE-100085](https://bugs.mojang.com/browse/MCPE-100085)）

性能与稳定性

* 修复了更改语言设置时可能发生的崩溃。
* 修复了抗锯齿设置设为1时打开成就界面可能发生的崩溃。（[MCPE-110164](https://bugs.mojang.com/browse/MCPE-110164)）
* 修复了`.mcstructure`文件保存的实体加载到世界中可能发生的游戏崩溃。（[MCPE-63387](https://bugs.mojang.com/browse/MCPE-63387)）
* 玩家在结构方块播放动画时传送离开不再会导致游戏崩溃。
* 修复了离开世界时可能发生的崩溃。
* 修复了有关市场上的世界加载受损生物群系的崩溃问题。
* 修复了使用代码连接功能时可能发生的崩溃。（[MCPE-113355](https://bugs.mojang.com/browse/MCPE-113355)）

常规

* 玩家再次能够加入视野距离设置为4或更小的服务器了。（[BDS-8855](https://bugs.mojang.com/browse/BDS-8855)）
* 恢复了在暂停和重启服务器时重新加入服务器的功能。
* 分屏的角色现在会储存，并且在重新加入游戏后保留玩家的角色。（[MCPE-58640](https://bugs.mojang.com/browse/MCPE-58640)）
* 更新了过时的加载界面提示。（[MCPE-98977](https://bugs.mojang.com/browse/MCPE-98977)、[MCPE-102293](https://bugs.mojang.com/browse/MCPE-102293)）
* 现在登录失败后游戏会提供更加实用的错误信息，同时还会显示错误代码。
* 解决了部分情况下无法将世界正确同步到云储存的问题（仅Xbox平台）。如果在同步世界时出现问题，请打开该世界，保存并退出，等待一段时间使世界重新同步到云储存中。
* 现在可以点击“下载模板”来正确地下载现有世界所缺少且需要的模板。
* 修复了“换床单啦”成就奖杯可以通过合成床来解锁的问题。

游戏内容

* 修复了玩家在打开潜影盒时会受到掉落伤害的问题。（[MCPE-105490](https://bugs.mojang.com/browse/MCPE-105490)）
* 玩家取消骑乘实体（如船）后不再会落入水和熔岩。
* 现在在所有用同一个种子创建的世界中，同一位置的战利品箱中总会以相同顺序生成相同的战利品。（[MCPE-72432](https://bugs.mojang.com/browse/MCPE-72432)）

生物

* 恢复了所有使用近战攻击的生物攻击其上方或下方目标的能力。
  * 仅影响大于或等于1.16.210的世界版本。
* 修复了鹦鹉能够无限向上飞行的漏洞。
* 修复了导致末影龙动画出现抖动的问题。（[MCPE-105892](https://bugs.mojang.com/browse/MCPE-105892)）
* 加入了生物取消骑乘其他实体的新逻辑规则。
  * 这也引入了一套更精确的实体高度检测机制，使得实体能够在不同高度处取消骑乘后落在不同位置。
* 修复了狐狸会不停地叼着甜浆果并无法吃甜浆果的漏洞。（[MCPE-70790](https://bugs.mojang.com/browse/MCPE-70790)）
* 修复了玩家能够在冒险模式下使用自定义刷怪蛋的漏洞。
* 现在矿车在玩家乘坐且未被渲染时会正确更新其效果（播放音效、玩家坐标）。（[MCPE-104044](https://bugs.mojang.com/browse/MCPE-104044)）

方块

* 现在用精准采集附魔工具破坏绯红菌核会掉落可放置的方块。
* 修复了部分市场上的世界有不正确的方块数据在Realms多人游戏中的移动端和PC端的世界生成的问题。
* 修改了干海带块的底面纹理，使其纹理上的“捆绳”和其他面对齐。（[MCPE-35476](https://bugs.mojang.com/browse/MCPE-35476)）
* 修复了下雪时在特定模拟距离的雪形成直线的问题。（[MCPE-73468](https://bugs.mojang.com/browse/MCPE-73468)）
* 现在水中爆炸的TNT会将生存模式的玩家推开。

物品

* 从流浪商人处获得的墨囊现在可以用于合成和堆叠。（[MCPE-101087](https://bugs.mojang.com/browse/MCPE-101087)）
* 红石粉的英文名称现在显示为“Redstone Dust”而不是“Redstone”。
* 玩家现在可以通过烧炼下界砖来获得经验值。（[MCPE-100030](https://bugs.mojang.com/browse/MCPE-100030)）

图形

* 修复了屏幕分辨率在调整窗口大小时可能会闪烁的问题。（[MCPE-69721](https://bugs.mojang.com/browse/MCPE-69721)）
* 修复了RTX世界中装有地图的物品展示框附着在透明方块上时产生的渲染问题。
* 减少了开启DLSS时透过水看鱼产生的重影。

辅助功能

* 修复了屏幕阅读器无法读取权限界面的标题的问题。
* 当鼠标光标在UI框架外面时，可用键盘调整使用滑块的设置。
* 当“聊天设置”菜单被打开时，屏幕阅读器会提示玩家相关内容。
* 修复了UI屏幕阅读器不会读取权限界面的权限开关选项的问题。
* 屏幕阅读器现在会读取Whisper和公告类消息。
* 现在屏幕阅读器会正确读取个人资料界面上的“编辑/创建角色“按钮的文字。
* 屏幕阅读器现在会在打开“聊天设置”时提醒玩家。
* 屏幕阅读器现在可以正确读取A/B或X/Y切换按键的名称。
* 修复了屏幕阅读器有时无法读取部分按键名称的问题。

用户界面

* 命令方块不再会将其命令替换为“###”。（[MCPE-106296](https://bugs.mojang.com/browse/MCPE-106296)）
* 改进了菜单过渡动画的平滑度（[MCPE-41772](https://bugs.mojang.com/browse/MCPE-41772)）
* 现在尝试把锁定的物品从容器中取出或放入容器时，将会出现警告。
* 更新了过时的加载界面提示。（[MCPE-98977](https://bugs.mojang.com/browse/MCPE-98977)、[MCPE-102293](https://bugs.mojang.com/browse/MCPE-102293)）
* 为支持光线追踪以及不支持光线追踪的平台加入了更多有用的视频设置信息。
* 金苹果和附魔金苹果现在被选中时会显示彩色的提示文本。（[MCPE-64427](https://bugs.mojang.com/browse/MCPE-64427)）
* 现在在配方表中选择工具和盔甲配方时会显示所选物品的背景。
* 现在鼠标停留在声音设置滑块会使该滑块变得高亮。
* 现在在窗口中拖动耐久度受损的物品会显示该物品的耐久度条。（[MCPE-105893](https://bugs.mojang.com/browse/MCPE-105893)）
* 修复了成就名称和描述未被翻译成所选择语言的问题。（[MCPE-85813](https://bugs.mojang.com/browse/MCPE-85813)）
* 检测到更改后，邀请屏幕上显示的跨平台好友的在线状态将会立即更新。（[MCPE-70004](https://bugs.mojang.com/browse/MCPE-70004)）
* 修复了更改语言设置后无法正确显示成就奖励的问题。
* 已拥有的和可购买的皮肤在离线时不再被分为不同的类别。
* 重新进入选项卡后，表情界面不再显示之前预览过的表情。
* 修正了使用控制器时的皮肤预览导航。
* 修复了市场“已拥有的包”界面缺失不兼容按键的问题。
* 修复了一些在滚动或清除市场过滤器时的界面问题。
* 选择是否在链接上下载资源包的时间限制由5秒提升至5分钟。
* 现在从添加好友界面返回游戏后邀请界面会正确刷新。

成就界面

* 现在默认使用新成就界面（除了VR、PS4平台或启用旁白功能的触控设备）。
* 移除了启用复述功能后的成就界面摘要面板的输入图例。
* 修复了滚动条能够隐藏在输入图例之后的问题。
* 修正了成就详细信息界面，其内容隐藏在输入图例之后。
* 更新了成就奖励框的大小。
* 更新了锁定成就的艺术图框。

命令

* `/`[`teleport`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/teleport)命令现在可以将目标实体传送至正确朝向。（[MCPE-35979](https://bugs.mojang.com/browse/MCPE-35979)）
* `/`[`summon`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/summon)命令现在会在生成事件中给出提示建议。（[MCPE-101112](https://bugs.mojang.com/browse/MCPE-101112)）
* 游戏规则`SendCommandFeedback`不再阻止传出消息。（[MCPE-95217](https://bugs.mojang.com/browse/MCPE-95217)）
* 在同一刻中多次执行`/`[`tickingarea`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/tickingarea) `add`或`/`[`tickingarea`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/tickingarea) `remove`命令不再导致出现关于所使用的常加载区域数量的错误消息。
* 玩家不再可以通过将所有独立常加载区域添加至同一刻中来超过所使用的常加载区域的最大数量。
* `/`[`setblock`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/setblock)命令现在可以设置灵魂灯笼的连接状态。（[MCPE-89609](https://bugs.mojang.com/browse/MCPE-89609)）
* `/`[`setblock`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/setblock)命令现在可以设置锁链的旋转状态。（[MCPE-105912](https://bugs.mojang.com/browse/MCPE-105912)）
* 修复了使用`/`[`clone`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/clone)命令复制大箱子后导致玩家无法互动的问题。（[MCPE-109119](https://bugs.mojang.com/browse/MCPE-109119)）
* 使用`/`[`clone`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/clone)命令复制相同类型的方块不再显示没有方块被复制。（[MCPE-83352](https://bugs.mojang.com/browse/MCPE-83352)）

技术性

* 现在马、驴、骡、骷髅马和僵尸马可被正确赋予自定义名称，且可使用其对应的`runtime_identifier`识别。
* 优化了活动对象使用`TemptGoal`时的性能。
* 在从市场下载的、1.11版本后创建的世界中，由刷怪笼生成的僵尸村民现在会正确地生成为V2僵尸村民，其被治愈后现在也能够正确地转化为V2村民。
* 修复了1.13.0中的`format_version`船升级到1.16.100的升级路径，以解决低于1.16.100的模板世界中的船没有重力的问题。
* 更新了基岩版服务器命令文档以重新加载和列出正确拼写的命令。（[BDS-2341](https://bugs.mojang.com/browse/BDS-2341)）
* 取消选择结构方块的结构名称文本框时，结构方块不再会自动保存数据。（[MCPE-101055](https://bugs.mojang.com/browse/MCPE-101055)）
* 现在使用材质状态“Blending”的实体在透明物体后面时会正确渲染。
* 实体被传送到世界的未加载区域时，不再删除该实体的记分板数据。
* 现在自定义方块被破坏后只会以默认的方块状态掉落了，不管是否使用精准采集。
* 禁用了自定义生物群系功能中的实体加载。
* 修复了数据驱动方块的UV会略微收缩且会导致纹理像素扭曲的问题。
* 修复了数据驱动方块被活塞推动后其无法正常工作的问题。



