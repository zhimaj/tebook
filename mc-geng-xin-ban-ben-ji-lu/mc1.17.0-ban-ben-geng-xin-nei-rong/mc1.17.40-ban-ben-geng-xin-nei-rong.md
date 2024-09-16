# MC1.17.40版本更新内容



{% hint style="info" %}
**【更新】1.17.40版本更新公告：**[ 洞穴与山崖](https://zh.minecraft.wiki/w/%E6%B4%9E%E7%A9%B4%E4%B8%8E%E5%B1%B1%E5%B4%96)（第四部分）

**更新版本：1.17.40 更新时间：2026-2-19 更新内容：**

**新内容：**
{% endhint %}



* [x] 本次更新为（第四部分）

更改\[ |]

常规\[ |]

[成就](https://zh.minecraft.wiki/w/%E6%88%90%E5%B0%B1)

* 为Windows 10 ARM的PC端启用了新成就界面。

[云](https://zh.minecraft.wiki/w/%E4%BA%91)

* 将漂浮高度由Y=128提高至Y=192。

[选项](https://zh.minecraft.wiki/w/%E9%80%89%E9%A1%B9)

* 移除了“显示边框效果”世界选项。

技术性\[ |]

数据驱动物品

* 更新了方块旋转组件文档。
* 为文档和方块组件的内容日志报错加入了需要的切换选项。
* 更新了BlockExplosionResistance文档。

图形

* 加入了在使用材质但未向渲染控制器提供所需纹理数量时出现的内容日志报错。

[Molang](https://zh.minecraft.wiki/w/Molang)

* 修复了query.item\_remaining\_use\_duration给出的结果会不正确缩放或倒置的问题（引擎版本1.17.30更改）。
* 为text + 3等在之前被忽略的表达式加入了新的编译错误（引擎版本1.17.40更改）。
* 现在包含大写字母的Molang表达式会被正确评估了。
* query.get\_equipped\_item\_name查询现在会正确识别海晶灯。（[MCPE-67893](https://bugs.mojang.com/browse/MCPE-67893)）
* 为1 + (9 10)等在之前被忽略的表达式加入了新的编译错误（引擎版本1.17.40更改）。

实验性\[ |]

本段落的内容需要开启[实验性玩法](https://zh.minecraft.wiki/w/%E5%AE%9E%E9%AA%8C%E6%80%A7%E7%8E%A9%E6%B3%95)中的“洞穴及悬崖”和“启用游戏测试框架”子选项后才可使用。

生物\[ |]

[驴](https://zh.minecraft.wiki/w/%E9%A9%B4)和[绵羊](https://zh.minecraft.wiki/w/%E7%BB%B5%E7%BE%8A)

* 现在会在[草甸](https://zh.minecraft.wiki/w/%E8%8D%89%E7%94%B8)中生成。

[狐狸](https://zh.minecraft.wiki/w/%E7%8B%90%E7%8B%B8)

* 现在会在[雪林](https://zh.minecraft.wiki/w/%E9%9B%AA%E6%9E%97)中生成。

[山羊](https://zh.minecraft.wiki/w/%E5%B1%B1%E7%BE%8A)

* 现在仅会在[积雪山坡](https://zh.minecraft.wiki/w/%E7%A7%AF%E9%9B%AA%E5%B1%B1%E5%9D%A1)、[裸岩山峰](https://zh.minecraft.wiki/w/%E8%A3%B8%E5%B2%A9%E5%B1%B1%E5%B3%B0)、[尖峭山峰](https://zh.minecraft.wiki/w/%E5%B0%96%E5%B3%AD%E5%B1%B1%E5%B3%B0)和[冰封山峰](https://zh.minecraft.wiki/w/%E5%86%B0%E5%B0%81%E5%B1%B1%E5%B3%B0)中生成。

[兔子](https://zh.minecraft.wiki/w/%E5%85%94%E5%AD%90)

* 现在会在[草甸](https://zh.minecraft.wiki/w/%E8%8D%89%E7%94%B8)和[积雪山坡](https://zh.minecraft.wiki/w/%E7%A7%AF%E9%9B%AA%E5%B1%B1%E5%9D%A1)中生成。

世界生成\[ |]

[生物群系](https://zh.minecraft.wiki/w/%E7%94%9F%E7%89%A9%E7%BE%A4%E7%B3%BB)

* 重新加入了[冰刺之地](https://zh.minecraft.wiki/w/%E5%86%B0%E5%88%BA%E4%B9%8B%E5%9C%B0)、[风蚀恶地](https://zh.minecraft.wiki/w/%E9%A3%8E%E8%9A%80%E6%81%B6%E5%9C%B0)、[丛林边缘](https://zh.minecraft.wiki/w/%E4%B8%9B%E6%9E%97%E8%BE%B9%E7%BC%98)和[热带高原](https://zh.minecraft.wiki/w/%E7%83%AD%E5%B8%A6%E9%AB%98%E5%8E%9F)。

[洞穴](https://zh.minecraft.wiki/w/%E6%B4%9E%E7%A9%B4)

* 现在主世界地底由两种岩层构成。
*
  * [石头](https://zh.minecraft.wiki/w/%E7%9F%B3%E5%A4%B4)作为Y=0以上的主要岩石生成。
  * [深板岩](https://zh.minecraft.wiki/w/%E6%B7%B1%E6%9D%BF%E5%B2%A9)作为Y=0以下的主要岩石生成。
  *
    * 在Y=-1至Y=-8处，石头逐渐向深板岩过渡；从Y=-8处开始，深板岩完全替换石头生成。
    * 生成于深板岩层的[矿石](https://zh.minecraft.wiki/w/%E7%9F%BF%E7%9F%B3)会被替换为对应的深层变种。
    * 深板岩层中不会生成[泥土](https://zh.minecraft.wiki/w/%E6%B3%A5%E5%9C%9F)、[闪长岩](https://zh.minecraft.wiki/w/%E9%97%AA%E9%95%BF%E5%B2%A9)、[花岗岩](https://zh.minecraft.wiki/w/%E8%8A%B1%E5%B2%97%E5%B2%A9)和[安山岩](https://zh.minecraft.wiki/w/%E5%AE%89%E5%B1%B1%E5%B2%A9)。

[溶洞](https://zh.minecraft.wiki/w/%E6%BA%B6%E6%B4%9E)

* 现在洞穴中的[草方块](https://zh.minecraft.wiki/w/%E8%8D%89%E6%96%B9%E5%9D%97)会在世界生成时替换为[石头](https://zh.minecraft.wiki/w/%E7%9F%B3%E5%A4%B4)。

[山地](https://zh.minecraft.wiki/w/%E5%B1%B1%E5%9C%B0)

* 加入了新的山地变种生物群系：[裸岩山峰](https://zh.minecraft.wiki/w/%E8%A3%B8%E5%B2%A9%E5%B1%B1%E5%B3%B0)。
*
  * [尖峭山峰](https://zh.minecraft.wiki/w/%E5%B0%96%E5%B3%AD%E5%B1%B1%E5%B3%B0)和[冰封山峰](https://zh.minecraft.wiki/w/%E5%86%B0%E5%B0%81%E5%B1%B1%E5%B3%B0)的未覆雪变种，而是裸露出[石头](https://zh.minecraft.wiki/w/%E7%9F%B3%E5%A4%B4)和条带状的[方解石](https://zh.minecraft.wiki/w/%E6%96%B9%E8%A7%A3%E7%9F%B3)地层。
  * 会替代前两种生物群系紧靠[温度](https://zh.minecraft.wiki/w/%E6%B8%A9%E5%BA%A6)较高的生物群系时生成。
* 调整了[草甸](https://zh.minecraft.wiki/w/%E8%8D%89%E7%94%B8)的植被生成以近似匹配[Java版](https://zh.minecraft.wiki/w/Java%E7%89%88)。
* [虫蚀石头](https://zh.minecraft.wiki/w/%E8%99%AB%E8%9A%80%E7%9F%B3%E5%A4%B4)现在会在新山地生物群系中生成。

[石岸](https://zh.minecraft.wiki/w/%E7%9F%B3%E5%B2%B8)

* 现在地表上有概率生成条带状的[沙砾](https://zh.minecraft.wiki/w/%E6%B2%99%E7%A0%BE)地层。

[![](file:///C:/Users/heaiz/AppData/Local/Temp/msohtmlclip1/01/clip\_image001.jpg)](https://zh.minecraft.wiki/w/File:1.18-exp1\_approximate\_ore\_distribution.jpg)1.17.40开启[实验性玩法](https://zh.minecraft.wiki/w/%E5%AE%9E%E9%AA%8C%E6%80%A7%E7%8E%A9%E6%B3%95)后的矿石分布

[矿石](https://zh.minecraft.wiki/w/%E7%9F%BF%E7%9F%B3)分布

* 调整了矿石分布以匹配[Java版1.18-exp1](https://zh.minecraft.wiki/w/Java%E7%89%881.18-exp1)。

[掠夺者前哨站](https://zh.minecraft.wiki/w/%E6%8E%A0%E5%A4%BA%E8%80%85%E5%89%8D%E5%93%A8%E7%AB%99)

* 现在会在新山地生物群系中生成。

[村庄](https://zh.minecraft.wiki/w/%E6%9D%91%E5%BA%84)

* 现在会在[草甸](https://zh.minecraft.wiki/w/%E8%8D%89%E7%94%B8)中生成。

常规

* 调整了主世界的生物群系分布、[河流](https://zh.minecraft.wiki/w/%E6%B2%B3%E6%B5%81)大小以及[地形特征](https://zh.minecraft.wiki/w/%E5%9C%B0%E5%BD%A2%E7%89%B9%E5%BE%81)，以改善玩家在主世界的游戏体验。
* 现在开启“洞穴及悬崖”选项后，旧区块的Y=0以下处会使用新的世界生成和洞穴生成。[\[2\]](https://zh.minecraft.wiki/w/%E5%9F%BA%E5%B2%A9%E7%89%881.17.40#cite\_note-2)
*
  * 之前版本升级过的区块的基岩层下方不会出现此更改。
  * 旧区块的基岩层会被替换为[深板岩](https://zh.minecraft.wiki/w/%E6%B7%B1%E6%9D%BF%E5%B2%A9)。
* 现在开启“洞穴及悬崖”选项后，旧的[超平坦世界](https://zh.minecraft.wiki/w/%E8%B6%85%E5%B9%B3%E5%9D%A6%E4%B8%96%E7%95%8C)会升级至新的世界建筑[高度](https://zh.minecraft.wiki/w/%E9%AB%98%E5%BA%A6)。
* 现在开启“洞穴及悬崖”选项的新超平坦世界会从Y=-64开始生成。

技术性\[ |]

GameTest框架

* 将方法succeedWhenBlockTypePresent重命名为succeedWhenBlockPresent。
* 修复了自定义实体的属性id会返回“未知”的漏洞。（[MCPE-137786](https://bugs.mojang.com/browse/MCPE-137786)）
* idnow属性返回的标识符字符串现在包含物品的命名空间。
* 更新了GameTest框架接口，并加入了新的SimulatedPlayer功能：
*
  * 为GameTest加入了SimulatedPlayer类型。此类型能够模拟玩家的各种行为，如移动、使用物品、与方块和实体交互等。
  *
    * 加入了函数spawnSimulatedPlayer(blockLocation: BlockLocation, name: string): SimulatedPlayer。
    * 加入了函数removeSimulatedPlayer(simulatedPlayer: SimulatedPlayer): void。
  * mojang-gametest.Test类型
  *
    * 修改了函数assertEntityInstancePresent(entity: Entity, blockLocation: BlockLocation, isPresent: boolean = true)的签名。
  * mojang-minecraft组件
  *
    * 组件库现可与玩家物品栏配合运行。
* GameTestSequence
*
  * 移除了thenWaitWithDelay方法。
  * 加入了thenWaitAfter(delayTicks: number, callback: () => undefined)方法。
  *
    * 一个延迟之后，每刻会执行指定的回调直到成功为止。回调过程中抛出的异常将结束序列执行。
* Player
*
  * 修复了位置属性会返回玩家不正确的高度的问题。
  * 加入了id属性。
* Block
*
  * 将getLocationwith方法替换为location属性。
  * 将getPermutationwith方法替换为permutation属性。
  * 将getTypewith替换为type属性。
  * 将isWaterloggedand和setWaterlogged替换为isWaterlogged属性。
  * 将getBlockDatawith方法替换为permutation属性。
  * 将isEmptywith方法替换为isEmpty属性。
  * 移除了canBeWaterlogged属性。
* BlockType
*
  * 将getNamewith替换为id属性。
  * 将canBeWaterloggedwith方法替换为canBeWaterlogged属性。
* BlockPermutation
*
  * 将getTypewith方法替换为type属性。

修复\[ |]

性能与稳定性

* 修复了使用角色创建器时可能发生的崩溃。
* 修复了在Realms上的世界槽位界面断开网络连接时可能出现的卡死问题。

常规

* 修复了Nintendo Switch玩家进入并离开世界后市场内容会下载失败的问题。
* 现在替换Realms世界时其世界设置会转移至Realms。

游戏内容

* 修复了下界传送门下方存在熔岩时，玩家传送至另一维度后会着火的漏洞。（[MCPE-28765](https://bugs.mojang.com/browse/MCPE-28765)）
* 改进了主世界地下的能见度剔除，以避免洞穴的尽头渲染为天空。（[MCPE-128372](https://bugs.mojang.com/browse/MCPE-128372)）
* 生存模式的玩家不再能在饥饿值满时进食了。（[MCPE-60807](https://bugs.mojang.com/browse/MCPE-60807)）
* 降低了紫晶洞生成在要塞附近的概率，即使如此生成也不会摧毁末地传送门。（[MCPE-129861](https://bugs.mojang.com/browse/MCPE-129861)、[MCPE-128799](https://bugs.mojang.com/browse/MCPE-128799)）
* 要塞在开启[实验性玩法](https://zh.minecraft.wiki/w/%E5%AE%9E%E9%AA%8C%E6%80%A7%E7%8E%A9%E6%B3%95)（洞穴及悬崖子选项）后不再会生成于错误位置或消失不见。（[MCPE-121708](https://bugs.mojang.com/browse/MCPE-121708)）
* 原版趋同：现在玩家可以在向上移动时使用鞘翅滑翔。（[MCPE-59580](https://bugs.mojang.com/browse/MCPE-59580)）

生物

* 使用水桶收集热带鱼后立即将其放出不再会使其失去颜色。（[MCPE-137158](https://bugs.mojang.com/browse/MCPE-137158)）
* 蜜蜂现在会在世界中以正确的数量生成。（[MCPE-132195](https://bugs.mojang.com/browse/MCPE-132195)）
* 非免疫火焰伤害的生物现在会避免进入火中。（[MCPE-23835](https://bugs.mojang.com/browse/MCPE-23835)）
* 村民不再能够快速地开关门。（[MCPE-28055](https://bugs.mojang.com/browse/MCPE-28055)）
* 制图师现在会在所有平台提供更加一致的新地图交易。
* 改进了部分生物在非完整方块上的寻路机制。（[MCPE-127381](https://bugs.mojang.com/browse/MCPE-127381)）
* 盔甲不再会在掠夺者和卫道士身上显示，但仍然会提供防御效果。（[MCPE-74242](https://bugs.mojang.com/browse/MCPE-74242)）
* 修复了使用旧世界资源包后，卫道士在没有攻击目标时仍会渲染其武器的问题。（[MCPE-123229](https://bugs.mojang.com/browse/MCPE-123229)）
* 现在会有更多的敌对生物在主世界地下生成。
* 修复了给视角外的生物连接拴绳时该拴绳不会渲染的问题。（[MCPE-63931](https://bugs.mojang.com/browse/MCPE-63931)）
* 铁傀儡现在仅会生成在固体方块上。（[MCPE-140145](https://bugs.mojang.com/browse/MCPE-140145)）

方块

* 下落的钟乳石现在会正确偏移以避免与实际碰撞箱之外的实体交互。（[MCPE-132772](https://bugs.mojang.com/browse/MCPE-132772)）
* 蜂巢现在会面朝南方生成。
* 细雪不再在过远距离观察时消失。（[MCPE-127565](https://bugs.mojang.com/browse/MCPE-127565)）
* 现在结构方块加载活板门时该活板门会正确旋转。（[MCPE-66933](https://bugs.mojang.com/browse/MCPE-66933)）
* 海草在世界生成期间不再会在睡莲下方生成，以避免其破坏睡莲。
* 将雪层放置在草方块上后不再导致其行为异常。（[MCPE-140659](https://bugs.mojang.com/browse/MCPE-140659)、[MCPE-140660](https://bugs.mojang.com/browse/MCPE-140660)）

用户界面

* 现在非触摸控制玩家骑乘动物时会显示正确的按钮提示。
* 现在对着带有格式化代码的告示牌彩色文本使用染料染色会覆盖掉之前的格式化代码。
* 修复在告示牌文本界面上换行时会丢失文本格式的问题。现在文本会一直显示其拥有的格式，直到输入重置文本代码或其他格式化代码为止。之前放置的告示牌不会因此更改。
* 更改了好友更换皮肤时通知的消息。（[MCPE-92772](https://bugs.mojang.com/browse/MCPE-92772)）
* 修复了部分导航UI中无法使用导航键或方向键进行控制的问题。（[MCPE-132826](https://bugs.mojang.com/browse/MCPE-132826)）
* 修复了禁用屏幕动画后暂停游戏进入成就界面时可能会出现错误消息的问题。（[MCPE-132269](https://bugs.mojang.com/browse/MCPE-132269)）
* 修复了一个用途不大的游戏规则选项被添加至世界设置界面的问题。（[MCPE-139025](https://bugs.mojang.com/browse/MCPE-139025)）
* 主菜单的登录按钮不再会与市场按钮重叠。
* 在标签标题和设置界面的文字转语音选项的“Tab”单词之间添加了空格。
* 在登录失败界面中加入了“更多信息”按钮。

Realms

* 现在创建新世界前的所有设置更改会在世界创建后转移至该世界。

角色创建器

* 调整了默认的Steve皮肤颜色以匹配默认Steve角色。（[MCPE-120818](https://bugs.mojang.com/browse/MCPE-120818)）
* 背景皮肤不再会遮挡更衣室界面的左右箭头了。
* 打开角色创建器的经典皮肤包时，侧边栏不再会被打开。
* 改进了角色创建器的导航路径，以使其始终切换至选定的角色创建器角色。（[MCPE-139022](https://bugs.mojang.com/browse/MCPE-139022)）
* 现在可以在游戏中为角色装备市场中的皮肤。

命令

* 使用目标选择器@e\[type=]时教育版物品不再会作为选择目标出现了。（[MCPE-78363](https://bugs.mojang.com/browse/MCPE-78363)）
* 开启了“需要红石”选项且“延迟时间”不为0的命令方块现在仅会延迟时间内接受到红石信号才会执行命令。（[MCPE-74281](https://bugs.mojang.com/browse/MCPE-74281)）
* 修复了文本长度改变时/scoreboard命令的侧边栏不会显示对齐的问题。
* 修复了不能使用/summon命令来生成经验球的问题。（[MCPE-130835](https://bugs.mojang.com/browse/MCPE-130835)）

技术性

* 修复了区块卸载时仅显示实体消失的问题。
* 修复了修改渲染控制器时动画会重新启动的漏洞。

&#x20;
