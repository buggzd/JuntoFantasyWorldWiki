---
description: 一个自定义史蒂夫外观的mod
---

# Yes Steve Model ！

## mod信息

mod版本：yesstevemodel-1.18.2-release-1.1.2

mod百科：[https://www.mcmod.cn/class/8616.html](https://www.mcmod.cn/class/8616.html)&#x20;

介绍视频：[https://www.bilibili.com/video/BV1A14y1c7pe](https://www.bilibili.com/video/BV1A14y1c7pe)&#x20;

文档：[http://page.cfpa.team/ysm/zh/](http://page.cfpa.team/ysm/zh/)&#x20;

作者：[https://space.bilibili.com/4435845](https://space.bilibili.com/4435845)

## 如何获取皮肤

2023年3月21日：目前为止YSM还没有公布官方模型汇总网站，只能通过各种渠道下载别人的分享模型。

1. b站-烈鸟比百：[https://space.bilibili.com/20510758](https://space.bilibili.com/20510758)
2. mcbbs-黑克勒Heckler：[https://www.mcbbs.net/home.php?mod=space\&uid=4907576\&do=thread\&view=me\&from=space](https://www.mcbbs.net/home.php?mod=space\&uid=4907576\&do=thread\&view=me\&from=space)

## 快捷键

* alt+y : 打开展示面板
* z ：表情轮盘

## 专属指令

模组全部采用 /ysm 开头的指令，均需要 OP 2 等级权限才可以使用。所有的指令添加了游戏内的提示功能，所有模型 ID 、玩家 ID 即可智能提示。

```xml
/ysm model reload
```

重载全部模型文件：同时还会将模型文件向所有客户端玩家全部同步一次；

```
/ysm model set <player> <model_id> <texture_id> [ignore_auth] 
```

将特定模型、材质赋予给某个玩家，最后的 ignore\_auth 参数是可选参数，当设置为 true 时，会无视模型授权，强制为玩家赋予模型；

```
/ysm play <player> <animation_name>
```

强制玩家播放 xxx 动画；

```
/ysm play <player> stop 
```

清除之前强制玩家播放的动画；

```
/ysm auth <player> all 
```

向玩家授权全部模型；

```
/ysm auth <player> clear
```

清除玩家所有授权模型；

```
/ysm auth <player> add <model_id> 
```

向玩家授权 xxx 模型；

```
/ysm auth <player> remove <model_id>
```

清除玩家授权的 xxx 模型；

```xml
/ysm export <model_id>
```

将某个模型导出成 ysm 专属模型格式。
