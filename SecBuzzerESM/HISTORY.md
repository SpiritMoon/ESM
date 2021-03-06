# Release History
# V0.3.17 (2020-08-21)
- 更新 Suricata updater, 輸出更詳細的內容!
- 更新 Suricata updater, 增加隨機 Sleep

# V0.3.16 (2020-08-21)
- 換上 python 版本的 Suricata updater
- 修改 fluentd syslog host 欄位名稱為 hostname 

# V0.3.15 (2020-08-20)
- 更新 classification.config (新增快篩規則中定義的類別)

# V0.3.14 (2020-08-20)
- 補上缺少的 classification.config

# V0.3.13 (2020-08-20)
- 掛載 Suricata classification、iprep

# V0.3.12 (2020-08-19)
- 修改 es replica, 解決 ES 不健康

# V0.3.11
- 更新ESM的「連線」與「離線」安裝文件

# V0.3.10
- Update_Suricata_rules.sh 修改為使用 env 內的 key
- 更新 Winlog AI module 版本

# V0.3.9
- 隱藏重複創建 docker network 噴出的 error

# V0.3.8
- 修正 Suricata 無法送資料到ES

## V0.3.7
- cron 補上 pipe line 
- 移除 ES ILM相關設定

## V0.3.6
- 移除 ETA1 AI module
- 將 Suricata 規則更新改為每十分鐘觸發

## V0.3.5
- 將 AI 模組 PacketAnalyze 恢復
- 將 AI 模組 Winlog 恢復
- 將 AI 模組 ETA1 恢復
- Install.sh 加上更新規則

## V0.3.4
- Suricata 同步更新 rules

## V0.3.4
- 增加 Suricata Updater 延時

## V0.3.3
- ES 改為 OSS 版
- ES 改為單節點
- 暫時移除 AI 模組

## V0.3.2
- :tada: repush to Github :sparkler:

## V0.3.1
- 修正 Suricata updater 無法更新

## V0.3.0
- 新增 esm network
- 新增 ETA1 AI module
- 新增自動更新 suricata rules

## V0.2.24
- 修改 CEF Log Parser 處理欄位內容夾帶 "|" 符號狀況

## V0.2.23
- 更新 Update_Suricata_rulues.sh 
- 調整 suricata.yml 為讀取所有 rule

## V0.2.22
- 修正 AI docker-compose 格式錯誤

## V0.2.21
- 將 Winlog 觸發時間改為一小時一次
- 關閉 OMP module 
- 關閉 AI 用 mysql & 管理工具
- 增加 compose.sh 啟動 AI module

## V0.2.20
- 新增 Winlog 模組
- 新增 Cronjob 定時觸發 Winlog 模組
- 新增自動移除 eve.json

## V0.2.19
- 新增 PacketAnalyze 模組

## V0.2.18
- 新增 Suricata 資料打入 ES 時間欄位

## V0.2.17
- 修正suricata.yaml檔 - eve檔案輸出格式錯誤

## V0.2.16
- 調整 Update_Suricata_rules.sh 檔案路徑

## V0.2.15
- Suricata 資料新增 ticket 欄位

## V0.2.14
- 修正 Suricata rules 檔重複 sid

## V0.2.13
- 修正 Update_Suricata_rules.sh 檔案路徑

## V0.2.12
- Suricata 資料新增 dump_status 欄位

## V0.2.11
- 上傳初版 Suricata 更新腳本

## V0.2.10
- 修改 eve.json rotate 的區間
 
## V0.2.9
- 修正 Suricata 讀取不到網卡

## V0.2.8
- 修正 Fluentd 沒將規則送到 ES
- 修正 Cron 腳本不會自動重啟

## V0.2.7
- 新增離線安裝腳本 & 打包腳本

## V0.2.6
- 修正 Top Suricata Rules 因檔案名稱相同覆蓋狀況

## V0.2.5
- 修改 Suricata 設定檔, 避免 Windows 無法存取 Log
- 將 Suricata Image 上傳到 Docker hub

## V0.2.4
- 將 MiniSOC 改為 SecBuzzerESM

## V0.2.3
- 修改 Suricata docker-compose.yml, 修正 Build 後讀不到網卡

## V0.2.2
- 更新 Top Suricata Rules (20200721)

## V0.2.1
- 將 WEB 需要的 API KEY 加入到 MiniSOC.env
- 移除 POC 用不到的檔案 (Fluentd cron 備份 raw log)
- 
## V0.2.0
- 調整 sucicata, 不會輸出 fast.log, suricata.log
- 移除 POC 用不到的檔案

## V0.1.0
- Init, Base on MiniSOC 1.0.8
- Install.sh 腳本加上防呆
- 移除 Fluentd raw log 輸出
- 移除 prepare.sh & 舊版 install.sh
- 將 WEB 服務讀取的網卡加MiniSOC.env
