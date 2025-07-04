---
navigation:
  parent: crazyae2addons_index.md
  title: 生物成型面板
  icon: crazyae2addons:mob_formation_plane
categories:
  - Mob Storage
item_ids:
  - crazyae2addons:mob_formation_plane
---
# 生物成型面板

生物成型面板是一类特殊的线缆子部件，能直接放出生物。它的工作方式和标准的成型面板类似，但它专门用于生成捕获的生物。和仅取出模式的存储总线比较相似，只不过只适用于生物。

## 使用方法

1. **放置面板**
   - 将其放置在ME线缆上，输出面需朝向空气，生物会在该处生成。

2. **配置生物过滤器**
   - 右击面板打开其GUI。
   - 向配置槽中放入生物键，以进行白名单过滤。
   - 安装**反相卡**后，过滤器会变为黑名单。

3. **安装升级卡**&nbsp;*（可选）*
   - **容量卡**可解锁更多过滤槽。

4. **生成条件**
   - 面板前方和**上方**的方块必须为空气。
   - 两者中有一者不符合即不会生成。

---

## 工作原理

- 每次ME网络收到匹配的生物时：
   - 生物成型面板会检查过滤器中是否指明了该生物，以及优先级是否足够高。
   - 若条件符合且前述位置均为空气，则面板会生成生物。
   - 一次生成最多可产生24个生物。