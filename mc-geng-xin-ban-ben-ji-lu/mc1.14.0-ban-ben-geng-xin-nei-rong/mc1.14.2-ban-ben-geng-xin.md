# MC1.14.2版本更新

{% hint style="success" %}
#### 【更新】1.14.2版本补丁更新公告：BC1.14.2

&#x20; 更新补丁版本：1.14.2\
&#x20; 更新时间：2024-4-23\
&#x20; 更新内容：
{% endhint %}

### 修复

修复了32个漏洞

当前版本的热修复漏洞

* [REALMS-2860](https://bugs.mojang.com/browse/REALMS-2860) — 更新游戏后出现“您必须更新游戏才能继续在此 Realm 进行游戏。”提示。
* [REALMS-2871](https://bugs.mojang.com/browse/REALMS-2871) — Kindle设备上的Realms问题。

崩溃

* 修复了游戏过程中出现的若干崩溃。
* 修复了Nintendo Switch加载世界时发生的若干崩溃。
* 修复了将指南针和带有玩家标记的地图放入合成槽中导致的崩溃。（[MCPE-57882](https://bugs.mojang.com/browse/MCPE-57882)）
* 修复了与其他生物一同进入下界传送门时发生的崩溃。（[MCPE-58568](https://bugs.mojang.com/browse/MCPE-58568)）
* 修复了转换带有装载烟花的弩的世界会发生的崩溃。
* 修复了在转换后的世界发生袭击事件时会发生的崩溃。
* 修复了PlayStation 4和Xbox One加载Extreme Speed Runner市场世界时会发生的崩溃。

常规

* 经典皮肤不再在重启游戏时恢复。（[MCPE-55278](https://bugs.mojang.com/browse/MCPE-55278)）
* 修复了无法在运行iOS 13的设备上导入`.mcworld`和`.mctemplate`文件的问题。
* 修复了在硬盘上安装的游戏无法加载LittleBigPlanet世界和纹理包的问题。
* 修复了Chroma Hills纹理包无法在Nintendo Switch上加载的问题。
* 当分屏玩家加入世界的同时有一名玩家退出，不会再卡在屏幕边缘了。

游戏内容

* 现在可以在两个蜂蜜块之间的缝隙中发射投掷物。
* 玩家不会再被蜂蜜块推/拉时不正常弹起了。（[MCPE-53815](https://bugs.mojang.com/browse/MCPE-53815)）

生物

* 修复阻止怪物在透明方块下生成的问题。（[MCPE-59682](https://bugs.mojang.com/browse/MCPE-59682)）
* 蜜蜂不再从着火的蜂巢或蜂箱中飞出。（[MCPE-53872](https://bugs.mojang.com/browse/MCPE-53872)）
* 通过提升优先级修复了驯服的狼不繁殖的问题。（[MCPE-59570](https://bugs.mojang.com/browse/MCPE-59570)）
* 修复了玩家肩上的鹦鹉不能正常通过世界转换的问题。
* 修复了掠夺者在世界转换后不攻击玩家的问题。
* 修复了玩家在世界转换后杀死掠夺者队长时不会获得不祥之兆效果的问题。

物品

* 三叉戟不再于蜂蜜块的侧面反复弹跳。（[MCPE-53626](https://bugs.mojang.com/browse/MCPE-53626)）
* 蜂蜜瓶现在会显示正确的物品提示。（[MCPE-61195](https://bugs.mojang.com/browse/MCPE-61195)）
* 未染色的潜影盒会在世界转换后恢复颜色了。（[MCPE-36744](https://bugs.mojang.com/browse/MCPE-36744)）

用户界面

* 在Nintendo Switch上购买Realms时会出现一个确认提示。
* 修复了在市场界面中调整与之前不同的窗口分辨率时可能导致文本重叠的问题。

命令

* 蜂巢和蜂箱使用`/`[`setblock`](https://zh.minecraft.wiki/w/%E5%91%BD%E4%BB%A4/setblock)命令放置时可以正确显示纹理了。
* 定义execute执行的位置不会截止detect参数了。

附加包

* 修复了导致行为包的动画有时无法在Android设备上显示的问题。（[MCPE-56117](https://bugs.mojang.com/browse/MCPE-56117)）
* 检测系统（用于远程攻击）现在会像往常一样计算所看的方向，使怪物能发现y轴上的目标了。
* 修复了阻止玩家被平滑传送和旋转的问题。
* 修复了动画控制器状态切换`on_exit`和`on_entry`事件时顺序颠倒的问题。
* 绑定到实体上的粒子效果的本地空间再次可以继承定位者的旋转角度了。
