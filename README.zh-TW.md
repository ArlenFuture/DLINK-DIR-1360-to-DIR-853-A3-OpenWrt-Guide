# DIR-1360 A1 刷成 DIR-853 A3 OpenWrt 非官方安裝教學

## 簡介  
這份教學是專門給 D-Link DIR-1360 A1 使用者，教你怎麼把它刷成 DIR-853 A3，因為這兩款設備的 PCB 設計完全一樣。完成後，這台路由器就能當作 DIR-853 A3 使用，並支援 OpenWrt 的韌體升級，讓功能更強大！  

## 安裝步驟  

### 1. 進入 Recovery 模式  
1. 確保路由器已接通電源。  
2. 長按路由器後面的 **RESET 按鈕**，直到橘燈開始閃爍。  

### 2. 使用 D-Link Recovery GUI 刷入改版韌體  
1. 打開瀏覽器，進入 D-Link Recovery GUI（通常為 `192.168.0.1`）。  
2. 下載由 Lucky1 修改過的 **DIR-853 A3 韌體**（已調整 Header）：  
   [韌體下載連結](https://forum.openwrt.org/t/adding-openwrt-support-for-dir-1360/98590/33)  
3. 在 Recovery GUI 上傳此韌體，並等待刷機完成。  

### 3. 後續韌體升級  
1. 刷機完成後，設備會直接變成 DIR-853 A3。  
2. 未來可以直接從 OpenWrt 官網下載對應的 DIR-853 A3 韌體進行升級：  
   [DIR-853 A3 OpenWrt 韌體下載](https://openwrt.org/toh/hwdata/d-link/d-link_dir-853_a3)  

## 實測結果  
目前測試在 OpenWrt 23.05.5：  
- **無線網路**：設定完成後需要重新開啟才會正常啟動。  
- **2.4G Wi-Fi**：持續存在問題，可能無法穩定使用。  
- **5G Wi-Fi**：正常運作，可穩定使用。  

## 注意事項  
- 本指南屬於非官方操作，刷機有風險，請自行承擔後果。  
- 建議刷機前備份好路由器的設定，防止意外發生。  

## 參考資料
- [DIR-1360 和 DIR-853 A3 PCB 詳細資訊](https://forum.dd-wrt.com/phpBB2/viewtopic.php?t=321874&sid=140829221456a3b23eae63c231ac58d9)  
- [Lucky1 修改固件討論串](https://forum.openwrt.org/t/adding-openwrt-support-for-dir-1360/98590/33)  
- [DIR-853 A3 OpenWrt 官網資訊](https://openwrt.org/toh/hwdata/d-link/d-link_dir-853_a3)  

## 貢獻  
發現問題或有建議嗎？歡迎透過 Issues 或 Pull Requests 回報，讓這份指南更完善！  

## 授權  
本專案採用 MIT 授權條款，詳情請參考 [LICENSE](LICENSE)。  
