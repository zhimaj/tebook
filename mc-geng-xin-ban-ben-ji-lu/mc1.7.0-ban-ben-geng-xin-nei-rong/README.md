# MC1.7.0版本更新内容

## 【更新】1.7.0版本更新公告：寒假新版本

#### 更新版本：1.7.0 更新时间：2021-12-23 更新内容：

新内容

#### 游戏内容

[记分板](https://zh.minecraft.wiki/w/%E8%AE%B0%E5%88%86%E6%9D%BF)系统

* 加入了基本的记分板功能。
* 追踪、编辑和显示每个玩家的特定项目。
* 通过使用`/`[`scoreboard`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/scoreboard)命令或者命令方块进行触发。

#### 命令格式

`/`[`scoreboard`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/scoreboard)

* 加入了基本的[记分板](https://zh.minecraft.wiki/w/%E8%AE%B0%E5%88%86%E6%9D%BF)功能。

`/`[`gamerule`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/gamerule)

* 加入`commandblocksenabled`规则。

#### 常规

[精选服务器](https://zh.minecraft.wiki/w/%E7%B2%BE%E9%80%89%E6%9C%8D%E5%8A%A1%E5%99%A8)

* 加入了_The Hive_服务器。

### 更改

#### 物品

常规

* 现在可以在[创造模式](https://zh.minecraft.wiki/w/%E5%88%9B%E9%80%A0%E6%A8%A1%E5%BC%8F)或[和平](https://zh.minecraft.wiki/w/%E9%9A%BE%E5%BA%A6#%E5%92%8C%E5%B9%B3%E9%9A%BE%E5%BA%A6)难度下吃东西了。

[紫颂果](https://zh.minecraft.wiki/w/%E7%B4%AB%E9%A2%82%E6%9E%9C)

* 从自然分类移动到物品分类。

#### 常规

[聊天](https://zh.minecraft.wiki/w/%E8%81%8A%E5%A4%A9)

* 聊天中所提到的玩家名称将会以黄色高亮。
* 聊天中输入@会显示玩家名称列表补全命令。

[商城](https://zh.minecraft.wiki/w/%E5%95%86%E5%9F%8E)

* 商城界面的顶部搜索、回到主页和查询已购项目更方便了。

[暂停菜单](https://zh.minecraft.wiki/w/%E6%9A%82%E5%81%9C%E8%8F%9C%E5%8D%95)

* “邀请好友”按钮被加入到设置里玩家列表的底部。
* 地图名称现在会显示在玩家列表的顶部。

### 修复

修复了77个漏洞

崩溃/性能

* 修复了游戏中发生的多次崩溃现象。
* 修复引雷三叉戟在雷雨天从发射器发射出并击中生物或玩家发生的崩溃。
* 修复在多个村民尝试开门或进门时破坏门发生的崩溃。（[MCPE-34742](https://bugs.mojang.com/browse/MCPE-34742)）
* 修复了Switch版应用128x资源包时发生的崩溃。
* 修复了当与制图师交易地图时所发生的崩溃。
* 加载资源包时游戏崩溃。
* 试图在存储空间不足的情况下回到Realms编辑界面里下载世界时游戏崩溃。

常规

* 修复了一个自定义皮肤漏洞利用，可通过几何上的透明皮肤在多人游戏模式获得优势。（[MCPE-37343](https://bugs.mojang.com/browse/MCPE-37343)）
* 在没有Switch在线会员的情况下禁用分屏功能时加入了额外的信息。
* 修复了分屏游戏下游客们和第一次加入游戏的顺序不同会生成不同的进度。
* Xbox One平台下现在能正确显示云端存档的列表。
* 修复了玩家在特定权限下无法破坏或放置方块。
* 超级马里奥混搭包在1.6.0以前的版本创建时无法打开世界。（[MCPE-37327](https://bugs.mojang.com/browse/MCPE-37327)）
* 修复了在Switch版里无法套用其余世界里的纹理包的问题。
* 修复了在Switch版里分屏玩家无法加入局域网世界的问题。
* 修复了在Switch版里无法登录Microsoft账号的问题。

游戏内容

* 打开物品栏或暂停菜单不再终止在梯子上潜行。（[MCPE-33209](https://bugs.mojang.com/browse/MCPE-33209)）
* 当使用触摸屏游泳时不再打破方块。（[MCPE-33470](https://bugs.mojang.com/browse/MCPE-33470)）
* 在船上现在可以丢弃物品。
* 抢夺III魔咒又一次增加了生物掉落物掉落的机会。（[MCPE-35307](https://bugs.mojang.com/browse/MCPE-35307)）
* 当玩家头部装备一个雕刻的南瓜时,玩家的标记会从其他玩家的定位器地图上消失。
* 玩家不再传送到在玩家渲染距离内被玩家的末影珍珠击中的载具或生物。
* 玩家不再在有限时间的边缘或者虚空里被困。
* 现在击退效果可以对生物造成击退伤害。（[MCPE-19222](https://bugs.mojang.com/browse/MCPE-19222)）

物品

* 在使用铁砧重命名一本附魔书并添加不兼容的附魔之后，附魔书不再丢失。
* 将带有忠诚的三叉戟投掷到虚空里时现在可以收回。
* 幻翼刷怪蛋现在可以使用选取方块键获得。
* 使用控制器的玩家骑乘矿车时现在可以丢弃物品。
* 当重新进入世界时，拴绳结不再消失。（[MCPE-33263](https://bugs.mojang.com/browse/MCPE-33263)）
* 附魔无限的弓轻微拉弓射出的箭不再立刻被玩家捡起。（[MCPE-35821](https://bugs.mojang.com/browse/MCPE-35821)）
* 重命名的刷怪蛋现在会生成重命名的生物。
* 燃烧的箭再次可以点燃TNT矿车。（[MCPE-35776](https://bugs.mojang.com/browse/MCPE-35776)）

生物

* 如果已驯服生物忘记了主人，它会坐下来等待有玩家与之互动，然后这个玩家将会成为新主人且不再需要重新驯服。（[MCPE-33152](https://bugs.mojang.com/browse/MCPE-33152)）
* 生物现在可以步行穿过灵魂沙和下界疣。（[MCPE-12719](https://bugs.mojang.com/browse/MCPE-12719)）
* 修复了骷髅马和僵尸马不会在一段时间后消失。（[MCPE-35215](https://bugs.mojang.com/browse/MCPE-35215)）
* 在船上对准前方的方块时，挖掘不再使得船上的马受伤。（[MCPE-30299](https://bugs.mojang.com/browse/MCPE-30299)）
* 从铁桶中放出热带鱼不再放出一条随机纹理的鱼而是最初捕获的那条。
* 拥有凋灵护甲的凋灵现在不会被投掷出的三叉戟造成伤害。
* 当溺尸乘船时不再有游泳动画。
* 在骑乘生物时，其余玩家不再能打开骑乘生物的物品栏。
* 除非它们刚好合适，否则生物再也不能在小缺口中生成。（[MCPE-31193](https://bugs.mojang.com/browse/MCPE-31193)）
* 末影人不再能生成于两个台阶之间的两格高的空间里。（[MCPE-28626](https://bugs.mojang.com/browse/MCPE-28626)）
* 现在可以对已经治愈的僵尸村民进行交易。（[MCPE-34603](https://bugs.mojang.com/browse/MCPE-34603)）
* 有鞍的猪现在当穿过2格高的水时，会把玩家从背上扔下去。

方块

* 玩家不可能在他们站着的地方放置方块。（[MCPE-31030](https://bugs.mojang.com/browse/MCPE-31030)）
* 海泡菜现在在生存模式下可以秒挖。（[MCPE-36250](https://bugs.mojang.com/browse/MCPE-36250)）
* 屏障不会被末影龙摧毁了。（[MCPE-34410](https://bugs.mojang.com/browse/MCPE-34410)）
* 刷怪笼在爆炸后不再掉落物品。（[MCPE-32657](https://bugs.mojang.com/browse/MCPE-32657)）
* 铁轨再次可以被流动的水破坏。

Realms

* 如果Xbox Live设置里不允许游玩Realms时，现在会弹出警告信息。
* 将本地世界上传至Realms时，现在会展示清晰的文本信息。

世界生成

* 梯子不再出现在村庄教堂结构的半空中。
* 结构不再能穿过海底神殿生成。

图形

* 修复了各种安卓设备上实体缺失部分身体模型。（[MCPE-34385](https://bugs.mojang.com/browse/MCPE-34385)）
* 在超平坦世界下，现在可以更容易看见水下的视野。（[MCPE-36078](https://bugs.mojang.com/browse/MCPE-36078)和[MCPE-35244](https://bugs.mojang.com/browse/MCPE-35244)）
* 在分屏里调整了弓和三叉戟的手持机制。
* 修复了当抛出附魔的激流的三叉戟时动画不会播放的问题。（[MCPE-34448](https://bugs.mojang.com/browse/MCPE-34448)）

音频

* 在iOS设备上收到系统通知之后声音会再度恢复。（[MCPE-15841](https://bugs.mojang.com/browse/MCPE-15841)）
* 现在可以正确地在游戏中播放凋灵生成时的音效。（[MCPE-35179](https://bugs.mojang.com/browse/MCPE-35179)）
* 旗帜现在有正确的放置和破坏的音效。（[MCPE-31188](https://bugs.mojang.com/browse/MCPE-31188)）
* 陆地生物现在可以在水下播放音效。

用户界面

* 修复了使用触摸输入时物品看和箱子中未正确堆叠的多个物品。（[MCPE-32347](https://bugs.mojang.com/browse/MCPE-32347)）
* 快捷栏里存在空槽位时，现在可以使用快速移动功能来将同种物品的不同个堆叠移入快捷栏里。
* 触摸屏的圆圈在打开物品栏或暂停菜单时冻结。（[MCPE-33895](https://bugs.mojang.com/browse/MCPE-33895)）
* 高亮铁砧的输出槽位时，移除了“拿起一半”的工具提示。
* 方块的“可以放置和“可以破坏”工具提示现在会显示它们的翻译。
* 修复了界面上错误的按钮位置。
* 修复了HUD显示格式化后的文本被截断的问题。
* 附魔台UI里的文本信息不再覆盖生成。

命令

* 游戏会话里的命令方块矿车现在会保存输入结果。
* 活板门在被`/`[`clone`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/clone)命令复制或移动时不再丢失方向。
* 命令的自动填充功能现在会将玩家的名字放入引号里。（[MCPE-34913](https://bugs.mojang.com/browse/MCPE-34913)）
* `/`[`teleport`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/teleport)命令现在会正确地传送玩家和他们正在骑乘的实体。
* `/`[`title`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/title) `<`_`实体`_`> subtitle`命令现在可以在显示了主标题后执行。（[MCPE-25685](https://bugs.mojang.com/browse/MCPE-25685)）

附加包

* 使用行为包来更改弹射物的发射位置时不再使得该弹射物丢失目标。
* 如果生物在行为包里被移除了所有运动组件，那么它们会停止移动。
* `can_float`组件现在能够在带有`minecraft:navigation.float`的飞行生物上运作。
