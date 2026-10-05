# 德州扑克平台源码、德州俱乐部、联盟、私人房 | Texas Holdem Poker Platform Source Code

[简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md) | [GitHub Pages](https://alibabama401.github.io/Texas-Holdem-Poker-Platform-Source-Code/)

一个面向多人扑克产品评估和服务端协议研究的公开资料库。仓库提供登录、用户状态和服务映射等 C++ 回调，以及俱乐部、联盟、私人房、SNG、MTT 与牌局记录相关 Protobuf 定义。

> **範圍說明 / 范围说明：** 本仓库是部分源码与协议参考，不是可直接编译或上线的完整平台。公开文件缺少完整依赖、构建脚本、数据库、服务入口、Unity 场景和后台前端。

## 产品截图

<table>
<tr><td width="50%"><img src="docs/assets/screenshots/dating_new.JPG" alt="多玩法大厅与房间列表" width="100%"><br><strong>多玩法大厅与房间列表</strong></td><td width="50%"><img src="docs/assets/screenshots/julebu.jpg" alt="俱乐部创建界面" width="100%"><br><strong>俱乐部创建界面</strong></td></tr>
<tr><td width="50%"><img src="docs/assets/screenshots/lianmeg.jpg" alt="联盟系统界面" width="100%"><br><strong>联盟系统界面</strong></td><td width="50%"><img src="docs/assets/screenshots/mtt02.jpg" alt="MTT 赛事盲注信息" width="100%"><br><strong>MTT 赛事盲注信息</strong></td></tr>
<tr><td width="50%"><img src="docs/assets/screenshots/sirenju.jpg" alt="好友私人牌局" width="100%"><br><strong>好友私人牌局</strong></td><td width="50%"><img src="docs/assets/screenshots/youxi.JPG" alt="德州扑克游戏界面" width="100%"><br><strong>德州扑克游戏界面</strong></td></tr>
</table>

## 可核验功能

- **C++ 回調 / 回呼：** 登錄/登入令牌、連接/連線映射、用戶/使用者資料、在線/線上狀態、房間狀態和退出處理。
- **俱樂部、聯盟與私人房：** 建立、加入、搜尋、審核、成員、職位、帳單、牌桌和聯盟訊息。
- **SNG 與 MTT：** 賽事房間、盲注、報名費、獎勵、排名、重購和退款欄位。
- **德州協議：** `dz.proto`、`GameRecord.proto` 與 `Friends.proto` 提供牌局、記錄和社交資料結構。
- **產品素材：** 12 張本地截圖和一個影片，展示大廳、俱樂部、聯盟、賽事、私人房與牌桌介面。

## Texas Hold’em 基本玩法

每位玩家獲得兩張私有底牌。翻牌、轉牌和河牌依序公開五張公共牌；各輪可根據規則過牌、跟注、加注或棄牌。玩家從七張可用牌中組成最佳五張牌。倉庫協議還包含 SNG 與 MTT 賽事相關欄位。

## 公开文件映射

| 公開檔案 | 可核驗內容 |
|---|---|
| `AsyncLoginCallback.*` | 登入結果、連線映射與狀態通知 |
| `AsyncGetUserCallback.*` | 裝置、平台、渠道、區域和機器人標記 |
| `AsyncUserServerMapCallback.*` | 線上、離線與房間狀態查詢 |
| `CommonStruct.proto` | 俱樂部、聯盟、賽事、私人房和金幣流水列舉 |
| `config.proto` | 房間、MTT/SNG、盲注、報名費、獎勵和俱樂部設定 |
| `dz.proto / GameRecord.proto` | 德州訊息欄位與牌局記錄結構 |

## 评估与使用

1. 先查看 `SOURCE-INVENTORY.md` 和實際公開檔案。
2. 補齊缺少的標頭檔、生成程式碼、依賴、服務實作、資料庫和配置。
3. 建立可重複建置、測試、安全和部署文件。
4. 請倉庫所有者釐清 `License.md` 中 MIT 與商用/保留權利文字的關係。
5. 正式使用前審核當地法規、平台規則、安全和遊戲公平性。

## Contact

Email: ttpoker40@gmail.com  
Telegram: [@alibabama401](https://t.me/alibabama401)

## 搜索关键词

德州撲克原始碼、德州撲克平台、C++ 撲克伺服器、Protobuf 撲克協議、撲克俱樂部、私人房、SNG、MTT、Texas Holdem source code。
