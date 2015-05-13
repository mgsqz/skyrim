# 人物

1. 部份指令效果需切換戰鬥姿勢一次後才會生效。
2. `forceav` 使用指定的數字， `modav` 正數為增加，負數為減少。
3. 更改人物屬性的指令前面加上 `player.` 開頭的話，就是是對玩家的人物使用，如果是 NPC 的話就要先點選後再使用。

## 屬性

指令|效果
---|--- 
player.sexchange | 變性
player.advlevel | 立刻升級
player.getlevel | 查看指定目標的等級
player.forceav health # | 增加生命上限
player.forceav stamina # | 增加耐力上限
player.forceav magicka # | 增加魔法上限
player.forceav healRate # | 生命恢復速度  預設 `0.7` (輸入 `10` 就算戰鬥中血很快就恢復滿 
player.forceav magickaRate # | 魔法恢復速度  預設 `3.0`
player.forceav staminaRate # | 耐力恢復速度  預設 `20.0`
player.forceav speedMult  # | 行走速度  預設 `100`
player.forceav carryWeight # | 負重
player.forceav dragonSouls #  | 龍魂數量
player.forceav weaponSpeedMult # | 調整武器的攻速倍數，預設 `1.0` ，最大 `2.0` (只有自己攻速會變) 。 數字不要一下就變化太大，可慢慢調高測試效果。調整後近戰類武器都會相同變更倍速，弓建議別超過 1.6 倍，不然會有打飛敵人等較誇張情況
player.setav rightItemCharge # | 右手附魔的 charge 數量 (裝備上武器是哪把就改的是哪把) 和附魔充能說再見
player.setav leftItemCharge # | 左手附魔的 charge 數量
player.setav paralysis # | 麻痺效果，預設 0 。取決你現在所有的帶麻痺屬性的裝備效果
player.setav invisibility # | 隱身效果，無該法術效果下預設 0 ，使用隱形術後數值1 改成5後 隱形術30秒效果消失後繼續保持隱形效果，持續多久未知
player.setav nightEye # | 夜視術效果等級
player.setav detectLifeRange # | 偵測生命類魔法的範圍，預設0
player.setav waterBreathing # | 水下呼吸
player.setav waterWalking # | 水面下沉速度，數值越高下沉越慢
player.setav wardPower # | ward 魔法吸收威力，預設 0
player.setav wardDeflection # | 魔法反射，預設 0
player.setav bowSpeedBonus # | 箭速獎勵，預設 `0.5` ，數值越大箭飛的越快
player.setav bowStaggerBonus # | 開弓獎勵，預設 `0.25` ，可能數值越大箭蓄力威力越大
player.setav absorbChance # | 吸取機率，各類吸紅，吸藍武器發出吸收類功能機率
player.setav unarmedDamage # | 拳擊傷害 預設攻擊力 4 ，獲得成就：你想吃一拳嗎？
player.setav meleeDamage # | 物理傷害（武器） 數值就是你的白字傷害
player.setav critChance # | 暴擊率，修改你現裝備武器的暴擊率
player.setav weaponSpeedMult # | 武器揮砍速度，取決於你的武器預設速度 例如匕首為 `1.35` 雙手武器為 `5` 別改太過分
player.setav leftWeaponSpeedMult # | 左手武器揮砍速度，同上
player.setav movementNoiseMult # | 腳步聲，採用負值，負數越大代表腳步越輕
player.setav bypassVendorStolenCheck 1 | 賣偷竊商品給任何商人
player.setav bypassVendorKeywordCheck 1 | 賣任何物品類型給商人
player.setav combatHealthRegenMult # | 戰鬥中生命恢復速率，預設 `0.7` ，意思就是每秒回覆你生命上限的 7%
player.setav reflectDamage # | 反射傷害，預設 0 ，效果未試驗，可能數值越高反射傷害越大
player.setav damageResist # | 護甲數值，物理護角，取決於你現在的裝備
player.setav poisonResist # | 毒抗 
player.setav fireResist # | 火抗
player.setav electricResist # | 電抗
player.setav frostResist # | 冰抗
player.setav magicResist # | 魔法抗性
player.setav diseaseResist # | 疾病抗性
player.setav ignoreCrippledLimbs # | 無視斷手斷腳，效果不明，預設0 

## 狀態

指令|效果
---|---
player.addItem a # | 添加開鎖器
player.addItem f # | 添加金錢
player.setav shoutRecoveryMult 0  | 龍吼無 CD
player.setCrimeGold 0 | 清掉自己頭上的賞金。要注意的是如果正被守衛追趕，則必須離開城市再回來指令才會生效。
player.payFine | 守衛停止攻擊，你頭上的賞金清除。可能會當機。
player.addShout xxxxx | 增加龍吼技能

## 強化法術效果

指令 | 系統 | 效果
---|---|--- 
player.modav illusionPowerMod # | 幻術系 | 加的是中招對像等級上限，如原本只有 20 級有效，改數字為 `100` 等於提高 100% 效果變成 40 級有效
player.modav alterationPowerMod # | 變化系 | 直接增加法術持續時間的 % 數，輸入 10 原本 50 秒的法術會變 55 秒
player.modav destructionPowerMod # | 毀滅系 | 加的是法術威力，原先傷害 50 輸入 `20` 會變傷害 60 [+20%]
player.modav conjurationPowerMod # | 召喚系 | 加的是召喚生物時間，同變化系的解說
player.modav restorationPowerMod # | 恢復系 | 效果提升同毀滅系的解說

## 射箭距離跟準度

打開 `skyrim.ini` 文件，在末尾新增：

```
[Actor]
fVisibleNavmeshMoveDist = 12288.0000

[Combat]
f1PArrowTiltUpAngle = 0.7
f3PArrowTiltUpAngle = 0.7

[Launcher]
bEnableFileSelection = 1
```

`[Actor]` 是修改射擊距離 (這個設定已超過肉視距離)
`[Combat]` 是修改準度(設定 `0.7` 後只需瞄準心的正中間，不需在計算拋物線)
`bEnableFileSelection` 是讓`載入MOD`可以點選
