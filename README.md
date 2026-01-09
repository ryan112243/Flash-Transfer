# Flash Transfer (快閃傳輸)

**Flash Transfer** 是一個基於 WebRTC 技術的單一 HTML 檔案 P2P 檔案傳輸工具。它設計用於在無需伺服器中轉的情況下，快速、安全地在裝置間傳輸檔案。所有數據僅暫存於瀏覽器記憶體中，分頁關閉即刻銷毀，確保極致隱私。

## ✨ 特色功能 (Features)

*   **⚡ 極速 P2P 傳輸**: 使用 WebRTC (PeerJS) 技術，檔案直接在裝置間點對點傳輸，不經過中間伺服器。
*   **🔒 端對端加密 (E2EE)**: 支援「私密模式」，檔名與說明皆經過 AES 加密，只有持有密碼的接收者能解鎖並下載。
*   **📂 單一 HTML 檔案**: 零後端、零安裝。只有一個 `.html` 檔案，雙擊即可執行，部署與分享極度容易。
*   **🧠 純記憶體暫存**: 檔案讀取後僅存在於 RAM (ArrayBuffer) 中，絕不寫入硬碟。一旦關閉分頁，資料完全消失，不留痕跡。
*   **🎨 現代化介面**: 
    *   專業深色模式 (Professional Dark Mode)。
    *   Windows 檔案總管風格的列表檢視。
    *   即時傳輸進度條。
    *   支援拖放 (Drag & Drop) 上傳。

## 🛠️ 技術棧 (Tech Stack)

*   **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
*   **P2P Connectivity**: [PeerJS](https://peerjs.com/) (WebRTC wrapper)
*   **Encryption**: [CryptoJS](https://cryptojs.gitbook.io/) (AES encryption)
*   **Icons**: Font Awesome

## 🚀 如何使用 (Usage)

1.  下載 `flash_transfer.html` 檔案。
2.  在瀏覽器中打開該檔案（建議使用 Chrome, Edge, Firefox 等現代瀏覽器）。
3.  **傳送者**:
    *   將檔案拖入中央區域。
    *   輸入檔案說明。
    *   選擇「公開模式」或「私密模式」(需設定密碼)。
    *   點擊「開始分享」。
4.  **接收者**:
    *   在同一個區域網路或互聯網環境下打開工具（確保能連接到 PeerJS server）。
    *   在列表中找到分享的檔案。
    *   點擊下載（私密檔案需輸入密碼解鎖）。

## ⚠️ 注意事項

*   由於使用公共 PeerJS 伺服器，建議用於非機密或已加密的檔案傳輸測試。
*   檔案大小受限於發送端與接收端的瀏覽器記憶體容量。

---
*Developed with ❤️ for secure and fast file sharing.*
