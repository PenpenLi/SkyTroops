## SkyTroops是飞行射击游戏，是plane框架的另一个游戏，素材比较完整，这次主要来试一下能不能做点牛逼的东西

## 使用新的层级结构，主要只有两个层，显示层和UI层，由默认摄像机对着，而游戏层是另外一个摄像机对着，显示层使用的是RenderLayer,这层可以进行后处理

## 12.7 -- 12.9
* 输入设置，使用虚拟摇杆,抽象成一个层(C)
* 敌人生成更改 (C)
* 子弹图更改 (C)
* 阻碍逻辑 (C)
* 自动发射子弹 (C)
* 加入背景 (C)
* 机体爆炸动画 (C)
* 加入摄像头和RednerTexture制作可以后处理的场景(C)(已经取消，太消耗性能)
* 主角加入飞行的尾气 (C)

## 12.10 --12.16
* ui基本完善 (C)
* loading 时间缩短 (C)
* 观看广告复活删除 (C)
* 所有敌机加入尾气(C)
* 加入全部飞机的资源 (C)
* 飞机根据不同等级会切换不同的图案(C)
* HUD显示炸弹(C)
* 炸弹逻辑 (C)
* 敌人的AI(3个) (C)
* 结算界面经验条 (C)
* 游戏icon以及游戏名字(android) (C)
* 敌机发射子弹逻辑 (C)
* 敌机拥有血量 (C)
* 主角血量显示 (C)
* DesignScene 加入各个敌人的生产逻辑 (C)
* 主角移动范围 (C)
* 炸弹逻辑 (C)
* 分数的规则 (C)
* 恢复和升级道具 (C)
* 放炸弹的逻辑优化 (C)
* 主角升级时候需要有个粒子特效 (C)
* 选择角色界面优化 (C)
* 设置本地保存数据，根据总分数解锁飞机 (C)
* 主页背景淡入(C)
* 暂停界面加入LayerColor (C)
* 解锁的UI (C)
* 根据分数积累经验条解锁飞机 (C)
* 道具的图像 (C)
* 主界面优化 (C)
* 暂停界面优化 (C)
* 加入恢复的道具和升级的道具(C)
* 子弹模式（根据不同等级子弹攻击力不同）(C)
* 一共6个关卡，关卡开始时候有显示文字，不loading加载关卡

## 优化

## 敌人Ai
* 移动型
1. 匀速直线移动 (C)
2. 直线到达距离特定高度时候加速直线移动 (C)
3. 绕弯追逐主角 (C)
4. 看见主角就发射子弹(C)
5. 发射散弹 (C)
6. 被打死发射一行子弹(C)
7. 被打死发射全场的散弹 (C)
8. 移动到主角位置发射子弹(C)
9. 发射两列子弹 (C)
10. 死亡时候有概率得到道具(C)
11. 被打死发射三个散弹(C)

* 发射子弹型
1. 简单直线发射 (4)
2. 主角在同一水平线发射 (C)
3. 移动到主角位置发射 (C)

* 发射子弹类型
1. 一个一个发射 （4)
2. 连续发射两个 (C)
3. 连续发射三个 (C)
4. 散发射 (C)
7. 发射的子弹会旋转

## 设计
* 三十秒，一分钟左右需要给予一定的反馈，可以是道具，升级，难度增大

## 待完善
* 子弹与敌机碰撞不精确(C)
* 游戏音乐和音效(C)
* 加入拖尾
* 游戏文字
* 多语言支持（中文和英文）
* 不续关的逻辑，广告五分钟后固定显示,最后一个解锁是解锁广告
