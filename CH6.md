# NPC 指令

大部份玩家能用的指令都可以在 NPC 上使用，但 `player` 要改成目標代碼，或用以下方法： 

1. 打開控制台，用游標點擊目標對象，獲取對象代碼
2. 用 `getav` 命令查看該人物當前的能力狀態， `modav` 或 `forceav` 則是修改
3. 需要減少的話將 `##` 輸入負數即可

## 同行

可隨意抓路人 NPC 使用，也可修改原本的護衛 NPC 能力。

指令 | 說明
---|---
setrelationshiprank player 1 | 啟用同伴指令
addfac 5C84D 1 | 擁有同伴選項
addfac 19809 1 | 到裂谷城酒吧找傳教，購買項鍊並戴上，再到要結婚對象面前輸入，即可打開婚姻選項
player.placeatme 00000007 | 複製主角自己當同伴 

## 為同伴量身打造技能

指令 | 說明
---|---
modav onehanded ## | 單手武器
modav twohanded ## | 雙手武器
modav marksman ## | 箭術
modav block ## | 格擋
modav heavyarmor ## | 重甲
modav lightarmor ## | 輕甲
modav sneak ## | 潛行
modav alteration ## | 變化魔法
modav conjuration ## | 召喚魔法
modav illusion ## | 迷幻魔法
modav restoration ## | 回復魔法
modav destruction ## | 毀滅魔法
modav lockpicking ## | 開鎖
modav pickpocket ## | 偷竊

至於技能點則無需手動添加，只要等級到了，他會自動擁有該等級可學的技能。

### 基本屬性

指令 | 說明
---|---
forceav health ## | 血量
forceav magicka ## | 魔法
forceav stamina ## | 體力
forceav healrate ## | 血量恢復
forceav magickarate ## | 魔法恢復
forceav staminarate ## | 體力恢復
forceav carryweight ## | 負重，數值直接指定，非增減
forceav speedmult ## | 移動速度，預設 `100` ，<br>改變一下攻擊姿態才可以看到效果

### 同伴性格與心情

指令 | 說明
---|---
setav confidence # | 更改同伴性格； `1` 膽小 / `2` 謹慎 / `3` 中庸 / `4` 勇敢 / `5` 蠻幹<br>弓法系設 `3` ，近戰系設 `4` 最佳
setav mood # | 更改同伴心情； `1` 平常心 / `2` 憤怒 / `3` 恐懼 / <br>`4` 悲傷 / `5` 歡樂 / `6` 驚訝 / `7` 迷惑 / `8` 噁心
setIgnoreFriendlyHits 1 | 不敵視指令 (防誤傷) ；指定的 NPC 生效後連續攻擊他也不會敵視你，<br>適用於同伴 NPC 或馬

## 魔法

指令 | 說明
---|---
addSpell xxxxxxxx | 加入代碼為 `xxxxxxxx` 的魔法
removeSpell xxxxxxxx | 移除代碼為 `xxxxxxxx` 的魔法

如果顯示 `not added` 表示 NPC 已學會。

代碼請參考[魔法](CH5.md) 。

## 為同伴打造裝備

指令 | 說明
---|---
showInventory | 查看同伴身上的裝備ID。<br>按鍵盤上 `Page Up` 和 `Page Down` 可以翻頁
addItem xxxxxx # | 添加裝備
removeitem xxxxxx #  | 移除裝備

要注意的是，預設裝備全部移除掉的話，系統會立即刷一批新的給他。因此必須得保留一件。

## 升級

1. 跟同伴對話，選擇「我們該分道揚鑣了。」
2. 打開控制台，點擊同伴獲取 ID (不是 baseID)
3. 輸入 `disable` ，此時同伴會消失
4. 接著輸入 `enable` ，消失的同伴又會在原地出現
5. 跟同伴對話，叫其跟隨。

需要注意的是，如果在同伴跟隨的狀態之下使用這個方法，同伴的能力值不會有絲毫改變，並且你給他的所有裝備都會消失。因此千萬記得遣散之後才進行操作。

## 產生怪物

用來屠城或讓怪物幫你清場。

指令 | 說明
---|---
placeAtMe xxxxx # | 需要點擊需要放置怪物的地點 (點著的地方必須顯示代碼) 

### 怪物代碼

代碼 | 名稱 | 代碼 | 名稱 | 代碼 | 名稱 | 代碼 | 名稱
---|---|---|---|---|---|---|---
F62EF | 裂谷男衛兵 | F62F0 | 裂谷女衛兵 | A27CC | 雪漫衛兵 | 559df | 風暴斗篷將軍
467bb | 風暴斗篷士兵 | 45BE0 | 帝國弓箭手 | 559e0 | 帝國將軍 | c0be5 | 巨人
B6234 | 長毛象 | 23ab6 | 雪劍齒虎 | 23ab5 | 劍齒虎 | 23abf | 冰狼
7871b | 狼人 | 23a8e | 雪熊 | c96c3 | 穴熊 | 2d1de | 骷髏
39d64 | 強盜首領 | 38a0f | 屍鬼首領 | 387c5 | 屍鬼 | 389ed | 屍鬼 (較強)
351c3 | 冰龍 | 1ca03 | 龍 | f77f8 | 血龍 | 2025a | 龍祭祀
21875 | 蟹 | 1b14f | 矮人機械蜘蛛 | 23aaa | 霜蜘蛛 | 23aab | 大蜘蛛
23abb | 雪巨魔 | 1b14e | 矮人百夫長 | 39cf9 | 強盜 | 1b151 | 烏鴉鬼婆
74f77 | 女巫 | 74f75 | 女巫 (強) | 4f4da | 男巫 | 4426f | 棄誓者弓箭手
442d4 | 棄誓者荊棘之心 | 23ab7 | 雪鼠 | 3383F | 瓦XX吸血鬼 | 33851 | 古代吸血鬼
10ddee | 惡魔公爵 | 16ff8 | 惡魔 | 23ab9 | 樹精 | a5600 | 查魯斯
23a8f | 大型查魯斯 | 23abd | 幽魂之母 | 45c5f | 冰法 | 45c60 | 火法
45c61 | 電法 | 23ab3 | 冰霜怒靈
