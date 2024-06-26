# MC1.16.6版本更新



> ## **【更新】1.16.6版本补丁更新公告：BC1.16.6**
>
> #### 更新补丁版本：1.16.6
>
> #### 更新时间：2025-1-23
>
> #### 更新内容：

### 更改

#### 方块

[告示牌](https://minecraft.fandom.com/zh/wiki/%E5%91%8A%E7%A4%BA%E7%89%8C)

* 现在可用[染料](https://minecraft.fandom.com/zh/wiki/%E6%9F%93%E6%96%99)对其文本染色，以同步[Java版](https://minecraft.fandom.com/zh/wiki/Java%E7%89%88)。

#### 技术性

GameTest框架

* 将活动对象的所有引用重命名为`Entity`。
* 将`BlockPos`重命名为`BlockLocation`。
* 在GameTest中加入了`startSequence`，允许对高级测试序列进行更好的控制。
* GameTest序列回调不再将`test`参数视为初始测试对象，因为其现在与整个测试一样有效。
* 更新了行为包以在使用其他本地模块时明确定义其依赖关系。
* 将`Blocks`快捷帮助中的部分英文单词更新为骆驼拼写法。
* 更新了仅包含原版方块的`Blocks`快捷命令。
* 加入了用于获取方块的`Blocks.get`函数，不存在方块时会返回到null。
* 加入了`BlockStates`，用于枚举所有的方块状态。
* 加入了`setState`，用于设置方块状态。
* 加入了`BlockPos`类型。
* 为`GameTest`模块加入了`ItemStack`类型。
* 加入了`Tags`，用于枚举内置标签。
* 更新了所有使用x，y，z坐标来执行的`BlockPos`函数。
* 现在注册GameTest时会公开填充。

移动预测

* 修复了第三方服务器上的弹射物会忽略服务器的移动数据包的问题。
* 现在当检测到玩家移动校正或异常时，服务器会根据其位置来调整其摔落距离。

网络传输

* 将UDP协议流的加密算法更改为AESGCM256。

### 修复

性能与稳定性

* 修复了一些游戏过程中可能发生的崩溃。
* 修复了玩家在第二个物品栏被占用时使用铁砧重命名地图发生的崩溃。（[MCPE-112905](https://bugs.mojang.com/browse/MCPE-112905)）
* 修复了进入下界传送门时投掷附魔之瓶发生的崩溃。（[MCPE-114793](https://bugs.mojang.com/browse/MCPE-114793)）
* 修复了Windows 10版中开启垂直同步后输入和操作出现延迟的漏洞。（[MCPE-98861](https://bugs.mojang.com/browse/MCPE-98861)）

游戏内容

* 修复了下界生物群系中的迷雾在某些资源包中无法正确渲染的问题。（[MCPE-111680](https://bugs.mojang.com/browse/MCPE-111680)）
* 现在具有访客权限的玩家死亡后会正确掉落物品。（[MCPE-47563](https://bugs.mojang.com/browse/MCPE-47563)）
* 修复了非访客分屏玩家在Xbox上会丢失数据的问题。（[MCPE-55815](https://bugs.mojang.com/browse/MCPE-55815)）

生物

* 修复了溺尸攻击时三叉戟会向后偏移的问题。（[MCPE-118213](https://bugs.mojang.com/browse/MCPE-118213)）
* 僵尸、僵尸村民、尸壳、掠夺者和卫道士现在会正确地手持盾牌。（[MCPE-98606](https://bugs.mojang.com/browse/MCPE-98606)）
* 现在一些人形怪物捡起盾牌后会将其持在副手上。
* 非不会被刷新的生物进入下界后不再会立即消失。

方块

* 弹射物现在能穿过结构空位。（[MCPE-103579](https://bugs.mojang.com/browse/MCPE-103579)）
* 改进了向楼梯、台阶及雪的侧面放置方块时的规则。
* 禁用轮廓选择后，活塞和黏性活塞的纹理不再会变黑。（[MCPE-53858](https://bugs.mojang.com/browse/MCPE-53858)）

辅助功能

* 现在在成就界面可以通过触摸输入来启用屏幕阅读器。
* 修复了使用VR时文本转语音会读取错误文本的漏洞。
* 修复了UI屏幕阅读器无法读取默认控制器的焦点和在线游戏未评级弹窗的漏洞。

用户界面

* 启用Xbox界面上的“寻找好友”按钮。
* 控制器现在可以在侏罗纪世界包中的NPC高级设置界面切换“按钮模式”选项。（[MCPE-66446](https://bugs.mojang.com/browse/MCPE-66446)）
* 现在市场上的“搜索结果”会在屏幕内不同部分之间正确刷新搜索内容。
* 使用VR时在全屏效果（如着火、进入下界传送门）发生后现在可以看到死亡界面。
* 修复了在方块附近打开菜单时封闭UI元素的半透明渲染问题。
* 现在选择个人资料界面上的特色优惠会正确进入完整的特色优惠列表。
* 现在葡萄牙语（巴西）的登录按钮文字在正确的位置上。
* 在设置界面的存储菜单中，文本现在使用较浅的颜色。
* 修复了应用资源包时按钮纹理缩放错误的问题。
* 在某些仅使用键盘的屏幕中启用了键盘返回按键。

命令

* 在关闭作弊后不再可以使用目标选择器选择自己。（[MCPE-92635](https://bugs.mojang.com/browse/MCPE-92635)）
* `/`[`clear`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/clear)命令现在可以为树苗应用`data`参数。（[MCPE-117889](https://bugs.mojang.com/browse/MCPE-117889)）
* 在同一串连锁型命令方块链中，添加了常加载区域后，再列出常加载区域会列出正确数量的常加载区域。
* `/`[`title`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/title)命令执行的屏幕标题不再会重复“%”。（[MCPE-51033](https://bugs.mojang.com/browse/MCPE-51033)）
* 现在`/`[`teleport`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/teleport)和`/`[`execute`](https://minecraft.fandom.com/zh/wiki/%E5%91%BD%E4%BB%A4/execute)命令配合使用时，会使用命令执行者所在的维度。（[MCPE-44104](https://bugs.mojang.com/browse/MCPE-44104)）

角色创建器

* 史蒂夫的裤子物品在没有穿戴鞋子物品时不再会给脚底添加颜色。
* 修复了多人游戏中的其他玩家的皮肤会变成Steve的问题。
* 现在在分屏模式下更改角色应该可以为所有本地玩家正确保存和刷新。
* 艾利克斯的衬衫物品与其他裤子物品搭配时不再显得破烂。
* 现在拥有“好耶！”表情会正确显示已拥有。（[MCPE-111165](https://bugs.mojang.com/browse/MCPE-111165)）

技术性

* 如果没有匹配的渲染控制器名称，则`render_controllers`中的标识符将被视为错误内容。
* 1.16.100版本前的实体json不再会给`minecraft:foot_size`弃用字段提供错误内容。
* 修改了`animation_controllers.json`中的条件以允许生物进入`wield_third_person_raise`。（[MCPE-118213](https://bugs.mojang.com/browse/MCPE-118213)）
* 修复了加载到世界中围绕“未处理的未知变量请求”会导致频繁出现MoLang错误的问题。
* 在部分世界中，暂停界面的玩家图标不再会变黑。内容创作者不再需要覆写`focus_border_frame.png`和`pause_screen_border.png`即可使其行为正常。
* 物品现在能够应用`transparentattachable`标签，以使穿戴该物品的玩家在第一人称视角下不渲染附加物品。
* 修复了村民V2在初始化时无法更新其MoLang变量的问题。
* 修复了新世界中仍会出现曾经执行失败的GameTest的问题。
