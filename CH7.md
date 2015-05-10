# NPC 代碼

## 找回同伴

指令 | 說明
---|---
prid xxxxx | 指定操作對象，等同用游標點選對象
moveTo player | 移動到玩家身邊
xxxxxx.moveTo player | 直接讓 xxxxxx 移動到玩家身邊
player.moveTo xxxxxx | 直接讓玩家移動到 xxxxxx 身邊

## 代碼分類

主分類：

名稱 | 說明
---|---
管家 | 領主分配的管家
傭兵 | 在各領地可花錢雇用的傭兵
朋友隨從 |  那些接受你的幫助後願意與你同行的NPC
15魔器 | 15魔器任務的NPC，需要對話或互動的，不包含魔神(山姆、圭文例外)
戰友團 | 
吟遊詩人學院 | 
法師學院 | 
盜賊公會 | 
黑暗兄弟會 | 
灰鬍子 | 包括四名灰鬍子與帕圖那克斯
刀鋒衛士 | 被梭默屠殺到剩兩人

子分類：

名稱 | 說明
---|---
隨從 | 
商人 | 
訓練師 | 
魔器 | 包含得到魔器後出現的眾多路人甲
官員 | 
領導者 | 公會領導者
公會任務 | 公會無限循環任務給予者
銷贓者 | 
敵人 | 有可能為或絕對為玩家敵人

## 管家 (包含子分類： [隨從])

代碼 | 名稱 | 子分類
---|---|---
A2C92 | Argis the Bulwark | [隨從]
A2C96 | Calder | [隨從]
A2C93 | Iona | [隨從]
A2C95 | Jordis the Sword-Maiden | [隨從]
A2C94 | Lydia | [隨從]

## Mod / DLC

代碼 | 名稱 | 子分類
---|---|---
1F001827 | Sofia | [隨從]
03002B74 | Serana | [隨從]

## 傭兵 (包含子分類： [隨從])

代碼 | 名稱 | 子分類
---|---|---
B9988 | Belrand | [隨從]
656E2 | Erik the Slayer | [隨從]
E1BA9 | Jenassa | [隨從]
B998C | Stenvar | [隨從]
B9986 | Marcurio | [隨從]
B9984 | Vorstag | [隨從]

## 朋友隨從 (包含子分類： [隨從] [魔器] [訓練師] [敵人])

代碼 | 名稱 | 子分類
---|---|---
1B13E | Adelaisa Vendicci | [隨從]
198B0 | Ahtar | [隨從]
1B092 | Annekke Crag-Jumper | [隨從]
28AD1 | Aranea Ienith | [魔器] [隨從]
1AA65 | Benor | [隨從]
5B688 | Borgakh the Steel Heart | [魔器] [隨從]
198FA | Cosnach | [隨從]
1B08D | Derkeethus | [隨從]
1BB8E | Eola | [魔器] [隨從] [敵人]
24280 | Erandur | [魔器] [隨從] [敵人]
1348C | Faendal | [訓練師] [隨從]
19930 | Ghorbash the Iron Hand | [魔器] [隨從]
A7360 | Golldir | [隨從]
CD92D | Kharjo | [隨從]
4B22E | Illia | [隨從]
19E1F | Lob | [魔器] [隨從]
19DF7 | Mjoll the Lioness | [隨從]
19E23 | Ogol | [魔器] [隨從]
1B084 | Roggi Knot-Beard | [隨從]
13491 | Sven | [隨從]
19E1B | Ugor | [魔器] [隨從]
91918 | Uthgerd the Unbroken | [隨從]

## 戰友團 (包含子分類： [隨從] [商人] [訓練師] [領導者] [公會任務] [官員])

代碼 | 名稱 | 子分類
---|---|---
1A697 | Aela the Huntress | [訓練師] [隨從] [公會任務]
1A6D6 | Athis | [訓練師] [隨從]
1A6A3 | Brill | 
1A683 | Eorlund Gray-Mane | [訓練師] [商人]
1A693 | Farkas | [訓練師] [隨從] [公會任務]
1A68F | Kodlak Whitemane | [領導者]
1A6DA | Njada Stonearm | [訓練師] [隨從]
1A6D8 | Ria | [隨從]
1A691 | Skjor | 
3BDE9 | Tilma the Haggard | 
1A6DC | Torvar | [隨從]
1A6A1 | Vignar Gray-Mane | [官員]
1A695 | Vilkas | [訓練師] [隨從] [公會任務]

## 吟遊詩人學院 (包含子分類： [訓練師] [領導者])

代碼 | 名稱 | 子分類
---|---|---
198D0 | Aia Arria | 
1F14D | Ataf | 
1027DB | Bendt | 
198CE | Giraud Gemane | [訓練師]
198D1 | Illdi | 
198CD | Inge Six Fingers | 
198CF | Jorn | 
198CC | Pantea Ateia | 
198CB | Viarmo | [領導者]

## 法師學院 (包含子分類： [隨從] [商人] [訓練師] [銷贓者] [領導者] [公會任務] [敵人])

代碼 | 名稱 | 子分類
---|---|---
1E7D8 | Ancano | [敵人]
1C1AB | Arniel Gane | 
1C1A4 | Brelyna Maryon | [隨從]
1C1A8 | Colette Marence | [商人] [訓練師]
1C1AA | Enthir | [銷贓者]
1C1A5 | Faralda | [商人] [訓練師]
J'1C1A3 | zargo | [隨從]
1C1B9 | Mirabelle Ervine | 
1C1A2 | Onmund | [隨從]
1C1A7 | Phinis Gestor | [商人] [訓練師]
1C1B8 | Savos Aren | [領導者]
1C23F | Sergius Turrianus | [公會任務] [訓練師]
1C1A1 | Tolfdir | [商人] [訓練師]
1C1B4 | Urag gro-Shub | [商人]

## 盜賊公會 (包含子分類： [商人] [訓練師] [銷贓者] [領導者] [公會任務] [敵人])

代碼 | 名稱 | 子分類
---|---|---
AC9E9 | Arnskar Ember-Master | [商人]
20545 | Brynjolf | 
D4FDA | Cynric Endell | 
1DA41 | Delvin Mallory | [訓練師] [公會任務]
19DFA | Dirge | 
3A1D6 | Etienne Rarnis | 
B4084 | Garthar | 
AC9E8 | Herluin Lothaire | [商人]
58F1A | Karliah | 
3BE26 | Maul | 
22651 | Mercer Frey | [領導者] [敵人]
49523 | Niruin | [訓練師]
B4085 | Ravyn Imyan | 
D4FE0 | Rune | 
C19A5 | Sapphire | 
AC9D7 | Syndus | [商人]
D4FDD | Thrynn | 
B882A | Tonilia | [銷贓者]
AC9EA | Vanryth Gatharian | [商人]
19DF9 | Vekel the Man | [商人]
28938 | Vex | [訓練師] [公會任務]
49535 | Vipir the Fleet | [訓練師]

## 黑暗兄弟會 (包含子分類： [隨從] [商人] [訓練師] [領導者] [公會任務] [敵人])

代碼 | 名稱 | 子分類
---|---|---
1BDE7 | Arnbjorn | [敵人]
1BDE8 | Astrid | [領導者] [敵人]
1D4BC | Babette | [商人] [訓練師]
9BCB0 | Cicero | [隨從] [敵人]
1D4BB | Festus Krex | [敵人]
1BDEB | Gabriella | [敵人]
3289A | Lis (蜘蛛) | [敵人]
1C3AD | Nazir | [訓練師] [敵人]
(無代碼) | Night Mother | [公會任務]
1C3AE | Veezara | [敵人]

## 灰鬍子 (包含子分類：無)

代碼 | 名稱 | 子分類
---|---|---
886B3 | Arngeir | 
886B4 | Borri | 
886B5 | Einarth | 
3C57D | Paarthurnax (龍) | [敵人]
886B6 | Wulfgar | 

## 刀鋒衛士 (包含子分類：無)

代碼 | 名稱 | 子分類
---|---|---
13485 | Delphine | 
19DFD | Esbern | 

## 15魔器 (包含子分類： [隨從] [魔器] [商人] [訓練師] [敵人] [官員])

### 阿祖拉之星、阿祖拉黑星 (Azura)

代碼 | 名稱 | 子分類
---|---|---
28AD1 | Aranea Ienith | [隨從] [魔器]
28AD5 | Malyn Varen (人，非屍骸) (盡量別使用) | [魔器] [敵人]
1E7D6 | Nelacar | [商人] [魔器]

### 黑檀鏈甲 (Boethiah)

無(沒有單個重要NPC)

### 卡拉威庫斯．維爾面具、悔恨之斧 (Clavicus Vile)

代碼 | 名稱 | 子分類
---|---|---
52535 | Barbas (狗) | [魔器]
3A19F | Lod | [商人] [魔器]
1C4EA | Sebastian Lort | [敵人] [魔器]

### 無限智典 (Hermaeus Mora)

代碼 | 名稱 | 子分類
---|---|---
2D4F2 | Septimus Signus | [魔器]

### 海爾辛之戒 、拯救者皮甲 (Hircine)

代碼 | 名稱 | 子分類
---|---|---
J'2ABC6 | Kier | [魔器]
1981A | Mathies | [魔器]
Sinding 6C1B8 (存在人、狼人兩種型態) [敵人] [魔器]
White Stag 90CE1 (鹿) [敵人] [魔器]

### 沃倫神鎚 (Malacath)

代碼 | 名稱 | 子分類
---|---|---
19E19 | Atub | [商人] [訓練師] [魔器]
3BC27 | Chief Yamarz | [敵人] [魔器]
19E1B | Ugor | [隨從] [魔器]

### 梅魯涅斯的刺刀 (Mehrunes Dagon)

代碼 | 名稱 | 子分類
---|---|---
240CE | Silus Vesuius | [敵人] [魔器]

### 黑檀利刃 (Mephala)

代碼 | 名稱 | 子分類
---|---|---
1A677 | Balgruuf the Greater | [官員] [魔器]
1A67E | Farengar Secret-Fire | [商人] [魔器]
1A67B | Nelkir | [魔器]

### 破曉者 (Meridia)

無NPC

### 莫拉格．巴爾釘鎚 (Molag Bal)

代碼 | 名稱 | 子分類
---|---|---
198F3 | Logrolf the Willful | [魔器]
A733C | Vigilant Tyranus | [敵人] [魔器]

### 娜米拉之戒 (Namira)

代碼 | 名稱 | 子分類
---|---|---
1BB8F | Brother Verulus | [魔器]
1BB8E | Eola | [隨從] [敵人] [魔器]

### 破法者 (Peryite)

代碼 | 名稱 | 子分類
---|---|---
8998C | Kesh the Clean | [魔器]
45F8E | Orchendor | [敵人] [魔器]

### 血腥玫瑰 (Sanguine)

代碼 | 名稱 | 子分類
---|---|---
1CB2B | Ennis | [魔器]
7A0EA | Gleda the Goat (山羊) | [魔器]
7A0E9 | Grok (巨人) | [敵人] [魔器]
1CB38 | Moira (烏鴉鬼婆) | [敵人] [魔器]
A96A0 | Sam Guevenne | [魔器]
263CD | Senna | [魔器]
1A69A | Ysolda | [魔器]

### 瓦巴杰克 (Sheogorath)

代碼 | 名稱 | 子分類
---|---|---
198DC | Dervenin | [魔器]
198C7 | Erdi | [魔器]
198C2 | Falk Firebeard | [官員] [魔器]
198C8 | Una | [魔器]

### 腐壞頭骨 (Vaermina)

代碼 | 名稱 | 子分類
---|---|---
24280 | Erandur | [隨從] [敵人] [魔器]
34200 | Thorek | [敵人] [魔器]
34201 | Veren Duleri | [敵人] [魔器]     