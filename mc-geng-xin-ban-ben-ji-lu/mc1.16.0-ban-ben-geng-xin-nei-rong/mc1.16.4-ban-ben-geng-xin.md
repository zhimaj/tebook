# MC1.16.4版本更新



{% hint style="info" %}
**【更新】1.16.4版本补丁更新公告：BC1.16.4**

更新补丁版本：1.16.4 更新时间：2024-11-14更新内容：
{% endhint %}

### 新内容

#### 游戏内容

[死亡消息](https://minecraft.fandom.com/zh/wiki/%E6%AD%BB%E4%BA%A1%E6%B6%88%E6%81%AF)

* 加入了以下死亡消息：
  * “\[玩家] 被 \[玩家/生物] 狙击了。”
    * 当玩家被[潜影贝](https://minecraft.fandom.com/zh/wiki/%E6%BD%9C%E5%BD%B1%E8%B4%9D)杀死时会出现。
  * “\[玩家] 被 \[玩家/生物] 吹了纸团。”
    * 应为“\[玩家] 被 \[玩家/生物] 的口水淹死了。”（原文中“spitball”被误译为“纸团”）
    * 当玩家被[羊驼](https://minecraft.fandom.com/zh/wiki/%E7%BE%8A%E9%A9%BC)杀死时会出现。

#### 常规



[菜单屏幕](https://minecraft.fandom.com/zh/wiki/%E8%8F%9C%E5%8D%95%E5%B1%8F%E5%B9%95)

* 加入了一个警告，提醒玩家正在使用过时的显卡驱动。

[选项](https://minecraft.fandom.com/zh/wiki/%E9%80%89%E9%A1%B9)

* 在音频设置中加入了更多设置以同步[Java版](https://minecraft.fandom.com/zh/wiki/Java%E7%89%88)：
  * 声音
  * 环境
  * 方块
  * 敌对生物
  * 友好生物
  * 玩家
  * 唱片机/音符盒
  * 天气



* 在视频设置中加入了“画质提升”、“光线追踪”和“光线追踪渲染距离”选项。
  * “画质提升”用于提高支持NVIDIA DLSS 2.0的GeForce RTX显卡的帧率。
  * “光线追踪”用于打开或关闭光线追踪。
  * “光线追踪渲染距离”用于控制光线追踪方块渲染距离。
  * 只有达到最低规格硬件的要求才能切换这些选项。

### 更改

#### 方块

[草径](https://minecraft.fandom.com/zh/wiki/%E8%8D%89%E5%BE%84)

* 重命名为土径。
* 现在当[泥土](https://minecraft.fandom.com/zh/wiki/%E6%B3%A5%E5%9C%9F)、[砂土](https://minecraft.fandom.com/zh/wiki/%E7%A0%82%E5%9C%9F)、[菌丝体](https://minecraft.fandom.com/zh/wiki/%E8%8F%8C%E4%B8%9D%E4%BD%93)或[灰化土](https://minecraft.fandom.com/zh/wiki/%E7%81%B0%E5%8C%96%E5%9C%9F)的上方没有方块时，对其顶部或侧面使用锹也能将其变为土径了。

#### 物品

[下界合金护腿](https://minecraft.fandom.com/zh/wiki/%E4%B8%8B%E7%95%8C%E5%90%88%E9%87%91%E6%8A%A4%E8%85%BF)

* 更改了穿着时的护腿模型纹理。

#### 游戏内容

[死亡消息](https://minecraft.fandom.com/zh/wiki/%E6%AD%BB%E4%BA%A1%E6%B6%88%E6%81%AF)

* 更改了以下死亡消息以匹配[Java版](https://minecraft.fandom.com/zh/wiki/Java%E7%89%88)：
  * “\[玩家] 被 \[玩家/生物] 射杀”
    * 取代“\[玩家] 被箭杀死”。
  * “\[玩家] 被 \[玩家/生物] 刺穿了”
    * 取代“\[玩家] 被 [三叉戟](https://minecraft.fandom.com/zh/wiki/%E4%B8%89%E5%8F%89%E6%88%9F) 杀死"”。
* 更改了以下死亡消息：
  * “\[玩家] 被 \[玩家/生物] 用火球烤死了”
    * 取代“\[玩家] 被 [烈焰人](https://minecraft.fandom.com/zh/wiki/%E7%83%88%E7%84%B0%E4%BA%BA) 杀死”。

#### 常规

[市场](https://minecraft.fandom.com/zh/wiki/%E5%B8%82%E5%9C%BA)

* 在市场中加入了一些能够显示资源包所支持的光线追踪功能的UI元素。（仅Windows 10平台）
  * 现在市场的资源包的购买界面中会显示是否支持光线追踪功能的标签。
  * 在尝试购买和/或下载需要启用光线追踪功能的资源包时，若没有达到最低规格硬件的要求，则会通知购买失败。

[选项](https://minecraft.fandom.com/zh/wiki/%E9%80%89%E9%A1%B9)

* 将音频设置中的“主音量”重命名为“主要”。

[RenderDragon](https://minecraft.fandom.com/zh/wiki/RenderDragon)

* 为Windows 10启用了RenderDragon。

[资源包](https://minecraft.fandom.com/zh/wiki/%E8%B5%84%E6%BA%90%E5%8C%85)

* 现在支持光线追踪。

地图制作和[附加包](https://minecraft.fandom.com/zh/wiki/%E9%99%84%E5%8A%A0%E5%8C%85)

* 为1.16.200更新了文档，并更新了资源和行为的模板。
* 更改了指定`block_type`时的`set_block`和`set_block_at_pos`，现在使用`BlockDescriptor`。
* 旧的命令现在使用先前的坐标而非现在的。
* 禁用Mipmap时将纹理图集的填充大小从0更改为1。

方块

* 加入了`query.cardinal_facing_2d`来获取水平方向而不会返回上或下的值。
* 在models/blocks文件夹里加入了放置方块模型的能力。
* 加入了物品触发器给互动的方块发送事件的能力（例如`on_use_on`）。
* 加入了查询方块和使用了`minecraft:on_use_on`的物品的互动面的能力。可通过`query.block_face`查询。

响应事件

* `add_mob_effect`和`remove_mob_effect`不再在传入有效的效果名时抛出内容错误。
* 为`remove_mob_effect`增加了文档来让创作者明白可以使用“all”值来移除一个对象的所有生物效果。
* 设置minecraft:inventory物品栏大小时必须新增与之匹配的槽位使服务器允许物品放置。
* 禁用游戏规则“showtags”时不再显示带有物品锁组件物品的工具提示。

### 修复

原版趋同

* 玄武岩不再会被恶魂火球破坏。（[MCPE-75252](https://bugs.mojang.com/browse/MCPE-75252)）
* 破坏玄武岩需要更长的时间了。
* 被爆炸破坏的龙蛋总是掉落为物品。（[MCPE-52632](https://bugs.mojang.com/browse/MCPE-52632)）
* 使用锹右键雪块时将不再破坏雪块。
* 更新了下界合金护腿的纹理。（[MCPE-103016](https://bugs.mojang.com/browse/MCPE-103016)）
* 潜行时不能再将缠怨藤放在堆肥桶方块上。（[MCPE-78973](https://bugs.mojang.com/browse/MCPE-78973)）
* 下界合金盔甲能够削减90%的击退魔咒效果了。（[MCPE-77430](https://bugs.mojang.com/browse/MCPE-77430)）
* 蜜蜂不会再飞离认领的蜂箱22格之外。（[MCPE-60252](https://bugs.mojang.com/browse/MCPE-60252)）

性能和稳定性

* 提升使用鞘翅飞行时区块的加载速度。（[MCPE-85614](https://bugs.mojang.com/browse/MCPE-85614)）
* 大量实时计划更新不再使游戏崩溃。（[MCPE-94942](https://bugs.mojang.com/browse/MCPE-94942)）
* 修复了一个在穿过传送门或在创造模式飞行时偶尔发生的崩溃。
* 修复了一个在世界中移动或飞行时偶尔发生的崩溃。
* 修复了一个在加载世界时偶尔发生的崩溃。
* 修复了在一些移动设备上恢复游戏暂停时无声的问题。（[MCPE-101027](https://bugs.mojang.com/browse/MCPE-101027)）
* 修复了使用Nintendo Switch尝试加载256x的资源包时引起的崩溃。
  * 系统会禁用选项并告知玩家不能选择此资源包。

常规

* 拥有创始者披风的玩家现在再次能够在更衣室中的披风选项卡中找到它了。

游戏内容

* 当自动合成在控制器中显示时才会显示物品预览，防止快速的合成表更新。
* 修复了玩家的手在视角晃动关闭时依然会摆动的问题。（[MCPE-79380](https://bugs.mojang.com/browse/MCPE-79380)）

生物

* 修复了生物和其他的实体会卡住且逐渐与它们的身体脱离的问题。（[MCPE-71243](https://bugs.mojang.com/browse/MCPE-71243)）
* 新的村民将不再认领已被认领的工作站点。（[MCPE-43071](https://bugs.mojang.com/browse/MCPE-43071)）
* 生物不再随机停止攻击和关注它们的对象了。（[MCPE-48144](https://bugs.mojang.com/browse/MCPE-48144)）
* 紧靠在一起的猪灵现在不会在掉落东西时捡起同一物品。（[MCPE-95644](https://bugs.mojang.com/browse/MCPE-95644)）
* 更新了僵尸猪灵的纹理来防止腰布的闪烁。（[MCPE-96793](https://bugs.mojang.com/browse/MCPE-96793)）
* 凋灵玫瑰中将不再有生物生成。（[MCPE-97331](https://bugs.mojang.com/browse/MCPE-97331)）
* 蜜蜂只能从[蜂箱](https://minecraft.fandom.com/zh/wiki/%E8%9C%82%E7%AE%B1)或[蜂巢](https://minecraft.fandom.com/zh/wiki/%E8%9C%82%E5%B7%A2)的正面出去。
* 当没有足够的空间容纳多个实体时，生物不再在固体方块之间来回传送。（[MCPE-101202](https://bugs.mojang.com/browse/MCPE-101202)）

物品

* 在创造模式下，对着[磁石](https://minecraft.fandom.com/zh/wiki/%E7%A3%81%E7%9F%B3)使用[指南针](https://minecraft.fandom.com/zh/wiki/%E6%8C%87%E5%8D%97%E9%92%88)将获得一个新的磁石指针。（[MCPE-96258](https://bugs.mojang.com/browse/MCPE-96258)）
* 荧光棒不再使用占位符纹理（教育版特性）。（[MCPE-45686](https://bugs.mojang.com/browse/MCPE-45686)、[MCPE-68417](https://bugs.mojang.com/browse/MCPE-68417)）

方块

* 热带雨林的可可豆现在会生成在正确的位置了。（[MCPE-102399](https://bugs.mojang.com/browse/MCPE-102399)）
* 尝试摆放告示牌不再会在要摆放的位置有装饰物时替换它了。
* 修复了一个当末地传送门框架被破坏时，末地传送门没有一并被破坏的问题。末地传送门以外的方块会保留在原位。

图形

* 在VR下重启游戏时将正确刷新已拥有的扩展包。

辅助功能

* 修复了屏幕阅读器无法阅读游戏主界面的问题。
* 修复了屏幕阅读器不会阅读游戏暂停界面按钮文字的问题。
* 修复了屏幕阅读器不会在邀请进入游戏的界面阅读菜单和按钮的问题。
* 修复了屏幕阅读器不会阅读个人资料和编辑角色界面标题的问题。
* 修复了使用文本转语音时暂停界面按钮编号错误的问题。
* 表情盘现在支持屏幕阅读器了
* 修复了一个屏幕阅读器无法在某些设备上更新阅读的问题。
* 修复了屏幕阅读器阅读聊天屏幕时有控制器图标时阅读不正确的问题。
* 屏幕阅读器现在会在文本转语音关闭时阅读聊天内容了。
* 修复了一些有关文本对比度的一些问题。
* 修复了一个服务器选项卡不会在没有登录Microsoft账户时正确文本转语音阅读的问题。
* 修复了若干文本转语音索引在主菜单中不正确的问题。
* 修复了用户界面控制不会在文本转语音为弹出模式时正确索引的问题。
* 降低了触屏UI第一行按钮的透明度，以提高可读性。

用户界面

* 修正了一些死亡消息。（[MCPE-30360](https://bugs.mojang.com/browse/MCPE-30360)、[MC-116558](https://bugs.mojang.com/browse/MC-116558)）
* 修复了更衣室中的纸娃娃不能被鼠标旋转的问题。（[MCPE-101210](https://bugs.mojang.com/browse/MCPE-101210)）
* “Classic Controls - Intense”字体颜色现在匹配在VR控制器菜单周围的文字了。
* 在合成方格中的预览物品现在有了不同的背景色，颜色取决于物品是否在物品栏中。
* 不管玩家的权限级别如何，权限菜单现在都能够使用控制器进入了。
* 在聊天设置中的\[X]按钮现在不会在使用控制器的时候显示了。
* 优化了个人档案界面，现在角色是可见的了，而且一旦被加载便可以被选中和修改它们了。
* 现在不会在玩家取消“需要购买记录”的对话框时要求购买Realms了。
* 角色创建器中的“Strawberry Blonde”颜色现在有了正确的名字了。（[MCPE-102674](https://bugs.mojang.com/browse/MCPE-102674)）
* 加载屏幕提示不再显示`tips.game.62`（No ID）了。
* 修复了在启用屏幕阅读器的情况下，将鼠标悬停在VR选项卡上时视觉焦点指示器在VR中消失的问题。
* 显示在人物列表的记分板可以于游戏暂停界面正常显示。（[MCPE-106012](https://bugs.mojang.com/browse/MCPE-106012)）

命令

* `/`[`playsound`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/playsound)命令可以使一定范围内的所有玩家听到声音。
* `/`[`effect`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/effect)命令中，状态效果的持续时间最多为1,000,000秒。（[MCPE-92916](https://bugs.mojang.com/browse/MCPE-92916)）
* 同一刻中执行的区域命令现在不允许重复添加有相同名称的区域。
* 执行`/`[`titleraw`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/titleraw)命令成功的占位文本现在不会发送给玩家了。（[MCPE-63618](https://bugs.mojang.com/browse/MCPE-63618)）
* `/`[`title`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/title)中的`FadeOut`参数不再被忽略了。

技术性

* 关闭了带宽优化来验证生物卡顿和延迟的问题是否被解决。
* 修复了自定义投掷物的动画。
* 修复了一个带有`set_data`的战利品表产生错误物品的错误。
* 修复了数据驱动的方块的面遮挡来解决单位方块透明与单位方块不透明的问题。
* 数据驱动的方块在物品栏中和手中时其顶部纹理不再被旋转180度。（[MCPE-63134](https://bugs.mojang.com/browse/MCPE-63134)）
* 修复了循环的数据驱动方块的方块刻队列顺序混乱的问题。该漏洞可能导致内存问题，增加负载与保存时间，并导致游戏周期性卡顿（无ID）。
* 修复了数据驱动方块以与actor相同的方式收缩UV的问题，以防止UV泄漏（无ID）。
* 修复了放置在区块边界上的尺寸大于1×1×1的数据驱动方块的一些剔除问题，并为较大的方块添加了内容警告。
* 修复了`query.cardinal_block_face_placed_on`无法与`on_player_placing`配合使用的问题。
* 修复了`minecraft:block_placer`组件中列出的方块无法正常工作的问题。
* 修复了事件发送至玩家后，玩家被重置导致其游泳和滑行时碰撞箱变小的问题。
* 修复了模板世界中自定义刷怪蛋的生成。
* MoLang的几何体，材质和纹理变量名称再次允许包含点。
* 具有物品锁定组件的物品不再导致合成配方显示无效的合成结果。
* 修复了`query.get_equipped_item_name`与重命名的物品一起使用后无法获得正确结果的问题。
  * 现在与原版版本号绑定，因此如果世界绑定到特定的原版版本，则会返回旧名称。
* 修复了物品无法放置在额外马具槽中的问题，但尚未修复所有装备的行为。
