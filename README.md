# GTQT-
GTQT入门指南

目录

* [下载与安装](#下载与安装)
  
* [游玩前注意事项](#游玩前注意事项)
  
游玩之前：整合包建议分配内存8g，分配内存过多可能导致游戏崩溃。在修改过资源包和光影后请重启游戏，否则会导致游戏帧数极低。

## 下载与安装
启动前的准备工作

下载地址&相关链接

https://www.mcmod.cn/modpack/590.html

https://www.mcbbs.net/thread-1437057-1-1.html

从前页的下载链接下载好curse格式的整合包之后（大小50MB），将其拖入PCL启动器等待其资源下载完毕，启动前检查JAVA路径，预留内存。

## 游玩前注意事项

1.关于更新以及备份存档，首先了解你的MC本体文件夹构成：

XaeroWaypoints 此文件夹存放着小地图标点信息，XaeroWorldMap 此文件夹存放着你的世界地图信息，Visualores 此文件夹存放着你的矿脉标点信息，你的备份存档存储在backups 文件夹。

更新时请注意保留以上文件夹再重装整合包。

2.如果你的存档突然消失，请不要紧张，你有两种办法挽回你的存档：

第一种：使用你的备份存档，通常存储在backups文件夹 内，将其转移到你的存档文件夹。

第二种：新建一个世界，拷贝你消失存档文件夹内的所有内容转移到新建的存档内，注意是清空后粘贴，不要覆盖。

引起存档消失的原因大部分来自于visualore与ScalingGUIs这两个模组冲突（触发条件，在非主世界维度使用探矿仪扫矿），如果不希望存档消失，删除其中一个模组即可。

如果你在使用终端探矿时遇到崩溃，请使用其他扫描仪器

3.如果你的存档出现地形生成问题（例如两次地图生成的一模一样，或者地形出现断层），在新建世界的时候不要使用相同的命名即可。

4.游戏优化攻略：适当调低角视场，在视频设置中选择流畅画质，关闭平滑光照，关闭动态光源，动画全关，渲染距离拉低（其余部分自行选择），不要开快速渲染！

5.开启光影，本整合包建议使用BSL 8.0.1以上的版本。请退出游戏在主界面更换光影，如果遇见游戏黑屏，重启游戏重复在游戏菜单界面更换光影的操作即可。

6.开局后先在第一章选择游戏难度！！！

请注意，里程碑和部分奖励只对easy难度开放，其余并无差别，且选择后不可修改。

如需要修改，请打开作弊模式，输入 添加阶段/gamestage add 【你的id】 (easy\hard)   

移除阶段/gamestage clear 【你的id】 (easy\hard)

7.商店部分出现部分物品贴图缺失系模组正常现象，内容暂未制作，并且此类物品均为后期内容，不影响现阶段游玩。

8.跑图卡顿：

RoguelikeDungeonsFnarEdition-1.12.2-2.4.4

BetterMineshaftsForge-1.12.2-2.2.1

bettercaves-1.12.2-2.0.4

也可以选择使用原版地形生成器。

删除以上三个模组，删掉之后跑图比原版还流畅。

9.任务如果遇到无法解锁，请查看任务前置是否完成，如何看任务前置

随便点开一个任务，你会在任务框顶部最左边图标的正下方有一个向左的三角，点击三角即可查看任务前置。

10.关于内网穿透显示 发生致命错误，链接终止
请按照如下步骤 单人模式打开或者创建你所需要的游戏存档，在生存模式下进入花园世界并且保证花园世界拥有一个FTB强制加载区块，3-5秒后重新尝试内网穿透。或者删除 实用世界 UtilityWorlds模组（这会导致花园世界消失，这也意味着你需要提前搬家，避免造成损失）

11.如何关闭左上角的小字
/igi disable
/igi config

12.如何关闭屏幕左侧的TOPC提示

非潜行状态手持readme右击（在你的阿卡什宝典里边）：

Needed：需要检测器才能显示信息；

Not Needed：直接显示，不需要检测器；

Extended：需要检测器才能显示详细信息。

潜行状态手持readme右击：

左侧可调整信息的显示位置，默认为左上角，点击左侧区域调整位置。

右侧可调整信息的显示样式和缩放。

13.区块加载器

打开位于右上角的FTB区块加载功能

单击区块：认领，在你的区块内默认防爆

SHIFT+点击：保持加载，无论玩家处于什么维度。

关于服务器区块问题。

请优先联系你的服务器管理员协调区块加载权限以及是否开启本功能。

14.请不要自行添加I18汉化，jech等模组，否则你将无法启动游戏

15.如果需要开启全屏，请在视频设置里选择 全屏：开

16.如果遇到内存清理卡顿，使用如下JVM参数：
-d64 -XX:+AggressiveOpts -XX:+UseConcMarkSweepGC -XX:+UseParNewGC -XX:+CMSConcurrentMTEnabled -XX:ParallelGCThreads=8 -Dsun.rmi.dgc.server.gcInterval=3600000 -XX:+UnlockExperimentalVMOptions -XX:+ExplicitGCInvokesConcurrent -XX:MaxGCPauseMillis=50 -XX:+AlwaysPreTouch -XX:+UseStringDeduplication -Dfml.ignorePatchDiscrepancies=true -Dfml.ignoreInvalidMinecraftCertificates=true -XX:-OmitStackTraceInFastThrow -XX:+OptimizeStringConcat -XX:+UseAdaptiveGCBoundary -XX:NewRatio=3 -Dfml.readTimeout=90 -XX:+UseFastAccessorMethods
