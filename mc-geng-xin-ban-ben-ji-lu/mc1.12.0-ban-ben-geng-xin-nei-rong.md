# MC1.12.0版本更新内容

{% hint style="success" %}
## 【更新】1.12.0版本更新公告：新版本

#### 更新版本：1.12.0 更新时间：2023-6-28 更新内容：

新内容
{% endhint %}

<details>

<summary><mark style="color:blue;"><strong>MC1.12.1补丁</strong></mark></summary>

#### 【更新】1.12.1版本补丁更新公告：BC1.12.1

&#x20; 更新补丁版本：1.12.1\
&#x20; 更新时间：2023-7-11\
&#x20; 更新内容：

### &#x20; 修复了4个漏洞

* 修复了若干可能在游戏时发生的崩溃。
* 修复了玩家在末地时加载世界卡在“生成世界”页面的问题。（[MCPE-49778](https://bugs.mojang.com/browse/MCPE-49778)）
* 修复了导致许多玩家无法在任天堂Switch上登录微软账户的问题。（[MCPE-34662](https://bugs.mojang.com/browse/MCPE-34662)）
* 末地不再会同时生成多条末影龙。（[MCPE-37590](https://bugs.mojang.com/browse/MCPE-37590)）

</details>

## 新内容

### 物品

[相机](https://zh.minecraft.wiki/w/%E7%9B%B8%E6%9C%BA)

* 重新加入了相机。
  * 只能通过使用`/`[`give`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/give)命令来获得。

## 命令格式

游戏规则

* 加入了`spawnradius`规则。
  * 允许指定玩家的生成半径。
  * 在世界设置中加入了新的“Respawn Radius”选项。
* 加入了`sendcommandblockfeedback`、`maxcommandchainlength`和`commandblockoutput`规则。
  * 和命令延迟选项相关。
* 加入了一些和[附加包](https://zh.minecraft.wiki/w/%E9%99%84%E5%8A%A0%E5%8C%85)、[地图](https://zh.minecraft.wiki/w/%E5%9C%B0%E5%9B%BE)制作相关的命令。

命名空间

* 于`/`[`give`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/give)命令加入`minecraft:`命名空间，以区分原版物品及附加物品。

`/`[`particle`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/particle)

* 加入了以下粒子:
  * `minecraft:dragon_death_explosion_emitter`
  * `minecraft:underwater_torch_particle`
  * `minecraft:dragon_destroy_block`
  * `minecraft:dragon_dying_explosion`
  * `minecraft:enchanting_table_particle`
  * `minecraft:falling_dust_concrete_powder_particle`
  * `minecraft:falling_dust_scaffolding_particle`
  * `minecraft:falling_dust_gravel_particle`
  * `minecraft:falling_dust_red_sand_particle`
  * `minecraft:falling_dust_sand_particle`
  * `minecraft:falling_dust_top_snow_particle`
  * `minecraft:huge_explosion_lab_misc_emitter`
  * `minecraft:ice_evaporation_emitter`
  * `minecraft:knockback_roar_particle`
  * `minecraft:lab_table_heatblock_dust_particle`
  * `minecraft:lab_table_misc_mystical_particle`
  * `minecraft:mob_block_spawn_emitter`
  * `minecraft:note_particle`
  * `minecraft:obsidian_glow_dust_particle`
  * `minecraft:phantom_trail_particle`
  * `minecraft:stunned_emitter`

### 常规

精选[服务器](https://zh.minecraft.wiki/w/%E6%9C%8D%E5%8A%A1%E5%99%A8)

* 允许[基岩版](https://zh.minecraft.wiki/w/%E5%9F%BA%E5%B2%A9%E7%89%88)[服务器](https://zh.minecraft.wiki/w/%E6%9C%8D%E5%8A%A1%E5%99%A8)上的内容登录。

物品ID

* 物品ID现在可以在[客户端](https://zh.minecraft.wiki/w/%E5%AE%A2%E6%88%B7%E7%AB%AF)和[服务端](https://zh.minecraft.wiki/w/%E6%9C%8D%E5%8A%A1%E7%AB%AF)同步。

[种子](https://zh.minecraft.wiki/w/%E7%A7%8D%E5%AD%90%EF%BC%88%E4%B8%96%E7%95%8C%E7%94%9F%E6%88%90%EF%BC%89)选择器

* 加入了10个种子。\[[需要测试](https://zh.minecraft.wiki/w/Talk:%E5%9F%BA%E5%B2%A9%E7%89%881.12.0)]

[闪烁标语](https://zh.minecraft.wiki/w/%E9%97%AA%E7%83%81%E6%A0%87%E8%AF%AD)

* 加入了新的闪烁标语：[\[2\]](https://zh.minecraft.wiki/w/%E5%9F%BA%E5%B2%A9%E7%89%881.12.0#cite\_note-2)
  * “All blocks covered!”
  * “feedback.minecraft.net”
  * “IT came from space.”
  * “Rainbow turtle?”
  * “Something funny!”
  * “I need more context.”
  * “Ahhhhhh!”
  * “Don't worry, be happy!”
  * “Water bottle!”
  * “What's the question?”
  * “Plant a tree!”
  * “Go to the dentist!”
  * “What do you expect?”
  * “Look mum, I'm in a splash!”

## 更改

### 方块

[海草](https://zh.minecraft.wiki/w/%E6%B5%B7%E8%8D%89)

* 更新了海草的纹理，使其与[Java版](https://zh.minecraft.wiki/w/Java%E7%89%88)匹配。

[命令方块](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4%E6%96%B9%E5%9D%97)

* 加入了自动完成。
* 加入了延迟选项。
  * 使用这个新的字段可以加入延迟。延迟的刻数是按[红石刻](https://zh.minecraft.wiki/w/%E7%BA%A2%E7%9F%B3%E5%88%BB)计算的。

[木桶](https://zh.minecraft.wiki/w/%E6%9C%A8%E6%A1%B6)

* 现在在[创造模式](https://zh.minecraft.wiki/w/%E5%88%9B%E9%80%A0%E6%A8%A1%E5%BC%8F)物品栏中有自己的位置，而不是位于“[箱子](https://zh.minecraft.wiki/w/%E7%AE%B1%E5%AD%90)”分类中。

[制图台](https://zh.minecraft.wiki/w/%E5%88%B6%E5%9B%BE%E5%8F%B0)和[讲台](https://zh.minecraft.wiki/w/%E8%AE%B2%E5%8F%B0)

* 调整并加入了界面提示。

[结构方块](https://zh.minecraft.wiki/w/%E7%BB%93%E6%9E%84%E6%96%B9%E5%9D%97)

* 现在在放置时有轮廓了。

### 生物

[流浪商人](https://zh.minecraft.wiki/w/%E6%B5%81%E6%B5%AA%E5%95%86%E4%BA%BA)

* 现在能打开[门](https://zh.minecraft.wiki/w/%E9%97%A8)。
* 加入了新的音效。
* [行商羊驼](https://zh.minecraft.wiki/w/%E8%A1%8C%E5%95%86%E7%BE%8A%E9%A9%BC)不再保护[流浪商人](https://zh.minecraft.wiki/w/%E6%B5%81%E6%B5%AA%E5%95%86%E4%BA%BA)。

[僵尸村民](https://zh.minecraft.wiki/w/%E5%83%B5%E5%B0%B8%E6%9D%91%E6%B0%91)

* 加入了新的音效。

[村民](https://zh.minecraft.wiki/w/%E6%9D%91%E6%B0%91)

* 村民的交易UI在玩家站得离村民太远时不会打开或关闭了。
* 村民现在会正确地寻找到自己的工作点了。
* 和玩家活跃交易中的村民不会在听到袭击铃声时逃跑或躲藏了。
* 加入了一个拒绝音效，用来指示村民不想交易（比如袭击时）。
* 被治愈后的村民会保留在变成[僵尸村民](https://zh.minecraft.wiki/w/%E5%83%B5%E5%B0%B8%E6%9D%91%E6%B0%91)前的职业。

[灾厄队长](https://zh.minecraft.wiki/w/%E7%81%BE%E5%8E%84%E9%98%9F%E9%95%BF)

* 现在用标签命令将普通[掠夺者](https://zh.minecraft.wiki/w/%E6%8E%A0%E5%A4%BA%E8%80%85)转换为灾厄队长时，[灾厄旗帜](https://zh.minecraft.wiki/w/%E7%81%BE%E5%8E%84%E6%97%97%E5%B8%9C)会正确显示。
* 灾厄队长现在会正确掉落[灾厄旗帜](https://zh.minecraft.wiki/w/%E7%81%BE%E5%8E%84%E6%97%97%E5%B8%9C)，即使世界被重新加载。
* [不祥之兆](https://zh.minecraft.wiki/w/%E4%B8%8D%E7%A5%A5%E4%B9%8B%E5%85%86)效果现在只会在击杀灾厄队长时给予，使用[弓箭](https://zh.minecraft.wiki/w/%E5%BC%93%E7%AE%AD)或者[药水](https://zh.minecraft.wiki/w/%E8%8D%AF%E6%B0%B4)造成非致命伤不会获得[不祥之兆](https://zh.minecraft.wiki/w/%E4%B8%8D%E7%A5%A5%E4%B9%8B%E5%85%86)效果。

## 常规

[附加包](https://zh.minecraft.wiki/w/%E9%99%84%E5%8A%A0%E5%8C%85)

* 附加包能用来加入新物品了。
* 生物事件可以在世界选项中启用/禁用了。
* 动画和粒子无需链接实体即可加入。
* 可以通过脚本修改物品栏、手持物品和装备栏了。
* 现在音效可以被动画事件触发了。
* 在脚本API中加入了新的`/`[`execute`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/execute)命令。
* 为与物品交互加入新的脚本事件，比如：
  * 捡起物品
  * 掉落物品
  * 持有的物品发生变动
* 加入了一次性动画支持，允许在实体上执行单个动画。
* 粒子发射器现在可以触发脚本事件。
* 更新actor事件的文档，以记录资源包中actor事件的客户端使用情况。
* “Add block”组件现在使用JSON模式。
* 加入了一个屏幕来查看内容日志错误。
* 日志屏幕可以使用Ctrl + H打开，或者进入设置→配置文件。
* 加入代码以允许在本地运行静态验证脚本。
* 现在可以通过脚本加入自定义方块。
  * 目前这仍是一个待完善的功能，更多的特性将会在未来的版本中加入。
* 现在只能通过额外的json脚本加入自定义方块。
  * 自定义方块只能使用/+命令放置。
* 加入了新的数据驱动粒子：
  * [羊驼](https://zh.minecraft.wiki/w/%E7%BE%8A%E9%A9%BC)吐口水
  * 大爆炸
  * 彩色火焰
  * [红石](https://zh.minecraft.wiki/w/%E7%BA%A2%E7%9F%B3)灰烬
  * 掉落的[沙子](https://zh.minecraft.wiki/w/%E6%B2%99%E5%AD%90)
  * [熔岩](https://zh.minecraft.wiki/w/%E7%86%94%E5%B2%A9)
  * [附魔台](https://zh.minecraft.wiki/w/%E9%99%84%E9%AD%94%E5%8F%B0)
  * [潮涌核心](https://zh.minecraft.wiki/w/%E6%BD%AE%E6%B6%8C%E6%A0%B8%E5%BF%83)
* 加入了新的数据驱动动画：
  * [狼](https://zh.minecraft.wiki/w/%E7%8B%BC)
  * [唤魔者](https://zh.minecraft.wiki/w/%E5%94%A4%E9%AD%94%E8%80%85)的尖牙攻击
  * [箭](https://zh.minecraft.wiki/w/%E7%AE%AD)
  * [潜影贝](https://zh.minecraft.wiki/w/%E6%BD%9C%E5%BD%B1%E8%B4%9D)导弹
  * [弓](https://zh.minecraft.wiki/w/%E5%BC%93)
  * [水](https://zh.minecraft.wiki/w/%E6%B0%B4)
* 更新文档以包含一个中端的更改部分。
* 基本物品相关事件已公开给脚本API。这包括:
  * `actor_acquired_item`
  * `actor_carried_item_changed`
  * `actor_dropped_item`
  * `actor_use_item`
  * `actor_equipped_armor`
* 基本物品栏事件已公开给脚本API。这包括:
  * `inventory_container`
  * `armor_container`
  * `hand_container`
  * `hotbar_container`
* 包含了新的方块事件和两个新的API来查询方块。这包括：
  * API：
  * `getBlock(Ticking Area, x, y, z)`
  * `getBlock(Ticking Area, PositionObject)`
  * `getBlocks(Ticking Area, x min, y min, z min, x max, y max, z max)`
  * `getBlocks(Ticking Area, Minimum PositionObject, Maximum PositionObject)`
  * 事件：
    * `block_destruction_started`
    * `block_destruction_stopped`
    * `piston_moved_block`
    * `player_destroyed_block`
    * `player_placed_block`
    * `executeCommand API`
  * 允许脚本API获取/+命令的结果。
* 事件数据API：
  * 允许开发者创建事件数据，注册并将其传递给事件函数。
* 更新了演示包。
* [生物群系](https://zh.minecraft.wiki/w/%E7%94%9F%E7%89%A9%E7%BE%A4%E7%B3%BB)的生成现在可以通过行为包定制。

音乐

* 现在在键盘显示在屏幕上时也会播放。

[菜单屏幕](https://zh.minecraft.wiki/w/%E8%8F%9C%E5%8D%95%E5%B1%8F%E5%B9%95)

* “商店”按钮现在被重命名为“市场”。

[闪烁标语](https://zh.minecraft.wiki/w/%E9%97%AA%E7%83%81%E6%A0%87%E8%AF%AD)

* 移除了有关[Notch](https://zh.minecraft.wiki/w/Notch)的闪烁标语：
  * “The Work of Notch!”
  * “110813!”

## 修复

修复了144个漏洞

崩溃

* 修复了游戏进行时出现的崩溃现象。
* Windows 10版下启动游戏时游戏崩溃。
* 加入Realms世界时，打开实体方块（例如[箱子](https://zh.minecraft.wiki/w/%E7%AE%B1%E5%AD%90)）导致游戏崩溃。
* 在Xbox上切换用户时游戏崩溃。
* 在海底神殿里与远古守卫者战斗时游戏崩溃。
* 加载游戏时游戏崩溃。
* 投掷鸡蛋或雪球时游戏崩溃。（[MCPE-40435](https://bugs.mojang.com/browse/MCPE-40435)）
* 与村民交易时游戏崩溃。
* 使用带有[忠诚](https://zh.minecraft.wiki/w/%E5%BF%A0%E8%AF%9A)魔咒的三叉戟时游戏崩溃。
* Nintendo Switch版在保存或加载游戏时游戏崩溃。（[MCPE-45862](https://bugs.mojang.com/browse/MCPE-45862)）
* Nintendo Switch版在暂停或继续游戏时游戏崩溃。
* 按下退出游戏按钮时游戏崩溃。
* 登录Xbox Live时游戏崩溃。
* 首次启动游戏时，选择皮肤使得游戏崩溃。
* 市场界面在加载内容时游戏画面冻结或崩溃。
* 游戏在检查此前已下载内容时崩溃。

性能

* 改进了打开物品栏时的性能。（[MCPE-27167](https://bugs.mojang.com/browse/MCPE-27167)）
* 改进了打开UI时的性能。
* 减少了带宽占用，使得客户端可以更快加载已有的区块。
* 提升了多人游戏下的区块加载性能。
* 改进了村庄和工作站点方块的性能。
* 改进了例如生物寻路AI之类的性能。
* 即将融化的霜冰导致巨大延迟。（[MCPE-39698](https://bugs.mojang.com/browse/MCPE-39698)）
* 末影人传送时的粒子不再使得性能下降，尤其是在末地里。
* 减少了加载资源包所需的内存大小。
* 缓存里的资源包不再导致Nintendo Switch版运行卡顿。（[MCPE-36976](https://bugs.mojang.com/browse/MCPE-36976)）

常规

* 移除了多余的Xbox Live登录提示。
* 消耗堆叠里最后一个物品时无法解锁相应的成就。
* “讨价还价”成就无法解锁。
* “僵尸医生”成就无法解锁。（[MCPE-46271](https://bugs.mojang.com/browse/MCPE-46271)）
* 在世界编辑界面里，下载的资源包不再被立刻启用。（[MCPE-33121](https://bugs.mojang.com/browse/MCPE-33121)）
* 当多个op在调整玩家权限时，现在会正确同步保存的选项。
* 改进了皮肤的漫游机制，使得重启游戏并登录后可以更快获取皮肤。
* 自定义皮肤不再需要重启游戏来启用。（[MCPE-37926](https://bugs.mojang.com/browse/MCPE-37926)和[MCPE-45476](https://bugs.mojang.com/browse/MCPE-45476)）
* “最近使用”界面里的皮肤现在可以重新使用。
* 不同的Xbox设备里现在会正确同步选项。
* 通过全局资源包选项里下载的资源包现在可以正确启用。
* 新购买的Realms世界现在可以在购买后立即显示。
* 在Xbox One里刷新Realms订阅时出现错误信息。（[REALMS-1686](https://bugs.mojang.com/browse/REALMS-1686)）

游戏内容

* 修复了部分与末地折跃门有关的漏洞，现在它可以正确将玩家传送到安全的位置。（[MCPE-43176](https://bugs.mojang.com/browse/MCPE-43176)、[MCPE-43177](https://bugs.mojang.com/browse/MCPE-43177)和[MCPE-19699](https://bugs.mojang.com/browse/MCPE-19699)）
* 村民购买物品时，不会拿走输入槽的第二个物品。（[MCPE-45506](https://bugs.mojang.com/browse/MCPE-45506)）
* 在Realms世界里，现在只有参与抵御[袭击](https://zh.minecraft.wiki/w/%E8%A2%AD%E5%87%BB)的玩家才能获得[村庄英雄](https://zh.minecraft.wiki/w/%E6%9D%91%E5%BA%84%E8%8B%B1%E9%9B%84)效果。
* 离开船后，玩家可以通过卡进方块里来透视世界。（[MCPE-42593](https://bugs.mojang.com/browse/MCPE-42593)）
* 使用触摸屏时，现在可以手持已经装填的弩来和方块交互。
* 玩家在水里取消游泳状态后可以透视方块。
* 被治愈的玩家现在会受到TNT的冲击。
* 重新加载世界时，射进方块的箭的位置会被保存。
* 区域效果云不再在时间被更改时生成大量药水粒子。（[MCPE-39595](https://bugs.mojang.com/browse/MCPE-39595)）

生物

* 狼身上的拴绳位置不正确。
* 已驯服的猫坐下时不再出现位置偏移。（[MCPE-44491](https://bugs.mojang.com/browse/MCPE-44491)）
* 部分僵尸村民的纹理丢失。
* 村民皮肤出现纹理深度冲突。
* 染色的皮革马铠不再能影响其他的马铠。（[MCPE-43230](https://bugs.mojang.com/browse/MCPE-43230)）
* 袭击里的卫道士现在能正确寻路。
* 重新进入存档后，凋灵会重复播放生成动画。（[MCPE-32415](https://bugs.mojang.com/browse/MCPE-32415)）
* 生物不再试图穿过酿造台。
* 加入了村民拒绝交易的音效（例如在袭击中）。
* 生物现在可以生成在双层台阶上。（[MCPE-30765](https://bugs.mojang.com/browse/MCPE-30765)）
* 修复了已驯服的猫的坐下模型。（[MCPE-41929](https://bugs.mojang.com/browse/MCPE-41929)）
* 僵尸村民的音效丢失。（[MCPE-43329](https://bugs.mojang.com/browse/MCPE-43329)）
* 新版僵尸村民在死亡信息里现在有了正确的名称。（[MCPE-45932](https://bugs.mojang.com/browse/MCPE-45932)）
* 生物在穿过梯子时不再被困在。（[MCPE-43034](https://bugs.mojang.com/browse/MCPE-43034)）
* 袭击里的唤魔者在寻找村庄时移速太快。
* 袭击参与者不再生成于树叶里。
* 处于交易状态中的村民不再主动跑离玩家，即使袭击的钟声响起。
* 已驯服的西服猫的纹理不正确。（[MCPE-43527](https://bugs.mojang.com/browse/MCPE-43527)）
* 转换自1.10的世界的村庄里的流浪猫不再能认领村庄里的床。（[MCPE-44299](https://bugs.mojang.com/browse/MCPE-44299)）
* 刷怪笼里的恶魂模型太大。
* 流浪商人的灰化土和珊瑚交易选项出现问题。
* 移除了流浪商人的沙子交易选项。
* 铁傀儡在村庄被摧毁后会主动移动至世界中心。（[MCPE-45509](https://bugs.mojang.com/browse/MCPE-45509)）
* 失业村民现在会遵循正确的日程安排和按时睡觉。
* 修复了部分市场地图里的苦力怕模型。

方块

* 部分方块只有在重启游戏后才能放置。
* 无法破坏霜冰。（[MCPE-41256](https://bugs.mojang.com/browse/MCPE-41256)）
* 流动的熔岩触碰水后再次会生成圆石。（[MCPE-43990](https://bugs.mojang.com/browse/MCPE-43990)）
* 红砂岩台阶的纹理不正确。（[MCPE-20677](https://bugs.mojang.com/browse/MCPE-20677)）
* 玩家在替换已经被交易过的村民绑定的职业站点方块时不再使得该方块的位置丢失。
* 被玩家使用的村民工作站点方块现在有了正确的音量。
* 脚手架不再能放置在潮涌核心上面。
* 钟的摆动方向不正确。（[MCPE-42469](https://bugs.mojang.com/browse/MCPE-42469)）
* 音符盒发出的音符粒子与音高不符。
* 砂轮现在能正确修复或合并损坏的物品。
* 耕地的侧面和底部纹理不正确。（[MCPE-42746](https://bugs.mojang.com/browse/MCPE-42746)）
* 烟熏炉的底部纹理不正确。（[MCPE-43944](https://bugs.mojang.com/browse/MCPE-43944)）
* 门和活板门的纹理不正确。（[MCPE-43173](https://bugs.mojang.com/browse/MCPE-43173)）
* 被活塞推动的可可果没有掉落物。（[MCPE-41868](https://bugs.mojang.com/browse/MCPE-41868)）
* 台阶和其他非固体方块现在再次能阻止草方块退化成泥土。（[MCPE-42975](https://bugs.mojang.com/browse/MCPE-42975)）
* 穿过绊线的流水不再使得出现积水现象。（[MCPE-36343](https://bugs.mojang.com/browse/MCPE-36343)）
* 现在可以使用喷溅药水或滞留药水敲击[钟](https://zh.minecraft.wiki/w/%E9%92%9F)。
* 堆肥桶发出的粒子位置不正确。
* 方块不能放置在红石矿石上面。（[MCPE-44305](https://bugs.mojang.com/browse/MCPE-44305)）
* 部分资源包里的流动水和熔岩纹理不正确。

物品

* 附有效率的镐现在能更快挖掘冰。（[MCPE-23648](https://bugs.mojang.com/browse/MCPE-23648)）
* 铁轨上的掉落物会阻止玩家放置矿车。
* 从酿造台取出的玻璃瓶不能正确堆叠。（[MCPE-42175](https://bugs.mojang.com/browse/MCPE-42175)）
* 物品栏已满时，不再能使用织布机来复制旗帜图案。
* 对着甜浆果丛使用“拾取方块”功能时现在会给予正确的物品。（[MCPE-41877](https://bugs.mojang.com/browse/MCPE-41877)）
* 对着草使用骨粉时现在会正确消耗骨粉。
* 不同生长状态的仙人掌现在都可用于烧炼为绿色染料。（[MCPE-42497](https://bugs.mojang.com/browse/MCPE-42497)）
* 在Realms世界里，使用去皮白桦木不再能合成金合欢木板。（[MCPE-44398](https://bugs.mojang.com/browse/MCPE-44398)）
* 物品展示框内的盾牌发亮。（[MCPE-41222](https://bugs.mojang.com/browse/MCPE-41222)）
* 更新了灾厄旗帜的纹理。（[MCPE-43233](https://bugs.mojang.com/browse/MCPE-43233)）
* 配方书里的旗帜合成配方现在会正确显示羊毛的颜色。
* 第一人称下的玩家进食时，不再使得手臂位置出现错误。（[MCPE-40135](https://bugs.mojang.com/browse/MCPE-40135)）
* 着色处理后的刷怪蛋放进物品展示框里时现在有了正确的大小。

世界生成

* 基岩版专用服务器或Realms世界里的部分方块生成错误。
* 调整了村庄里的工作站点方块数量。

用户界面

* 更新了制图台UI里锁定地图时出现的玻璃纹理。（[MCPE-43314](https://bugs.mojang.com/browse/MCPE-43314)）
* 调整了在安卓设备里使用经典UI时的制图台的UI大小。
* 在制图台UI里按下控制器Y按钮现在会给予正确数量的输出物品。
* 为控制器加入了讲台里的按键提示。
* 在交易界面里被拆分的一组物品现在仍会算进总交易数量里。
* 游戏指南里的制图台选项现在会指向正确的位置。
* 杀死行商羊驼不再使得它的物品栏被打开。
* Nintendo Switch版里玩家调整网络设置后不再出现多次提示。
* “总是白天”选项在启用时显示错误。（[MCPE-43304](https://bugs.mojang.com/browse/MCPE-43304)）
* 成就界面现在会再次显示玩家达成该成就的日期。
* “邀请好友”按钮不再能在精品服务器里起作用。
* 在启用文本转语音功能后，回到游戏选项界面里时现在正确选择此前已选的选项栏。
* “滚轮滚动”按钮现在只会在VR的设置选项里显示。
* “滚轮滚动”按钮现在只会在VR的设置选项里显示。
* 市场搜索界面现在会显示正确的资源包图标。
* 在已经浏览过相关内容后，“新！”标签现在会正确去除。
* 市场里的促销内容不会显示价格减少百分比。

命令

* 改进了使用命令的目标选择器。
* 移除了`/`[`give`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/give)命令里的`tile`前缀。（[MCPE-44667](https://bugs.mojang.com/browse/MCPE-44667)）
* 移除了物品的`tile`前缀来实现命名规则一致性。
* 使用命令时，创造模式物品栏里没有出现的方块或实体刷怪蛋不再需要输入`minecraft:`命名空间前缀。
* 使用命令清除浮漂实体后，玩家不再需要右键点击两次才能抛出新的浮漂。
* 同时杀死骑乘的实体和骑乘者时不再使得骑乘者重生。
* `/`[`testforblock`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/testforblock)命令不会对部分修改后的物品本地化名称起作用。

附加包和脚本引擎

* 行为包模板现在再次包含`spawn_rules`文件夹。
* 移除了旧的计时器组件并加入了全新的、不会继承此前的值的计时器组件。
* 自定义水下生物现在可以自然生成。
* 自定义实体现在会重新评估当前目标的有效性。
* `getBlocks`现在会返回方块对象的三维数组。
* 修复了脚本导致玩家悬空的漏洞。
* `ScriptAttackComponent`和`ScriptCollisionBoxComponent`现在会正确获取修改日期。
* 现在可以对非原版实体使用“拾取方块”按键。（[MCPE-38205](https://bugs.mojang.com/browse/MCPE-38205)）
* 在游戏里循环运行的函数现在需要Game Master权限，而不是玩家权限。
  * 为`ServerCommandOrigin`加入了新的构造参数以便管理者可以创建更新权限的实例。
* 玩家的位置现在取决于玩家的腿部位置，与其余生物一致。
* 碰撞箱和攻击组件现在会给予正确的日期。
