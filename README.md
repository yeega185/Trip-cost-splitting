# TripSplit - 旅行分帳系統 💰

![Project Status](https://img.shields.io/badge/Status-Active-success)
![Tech Stack](https://img.shields.io/badge/Stack-HTML%20%7C%20Tailwind%20%7C%20Firebase-blue)

一個現代化、響應式的旅行記帳與分帳網頁應用程式。專為團體旅遊設計，能夠即時記錄開銷，並透過演算法自動計算出「最少轉帳次數」的結清方案，解決多人旅遊算錢的煩惱。

## ✨ 功能特色

* **👥 參與者管理**：彈性新增旅伴，支援權重（份數）設定。
* **📝 即時記帳**：清楚記錄每一筆消費的支付者與分攤者。
* **📱 現代化介面**：使用 Tailwind CSS 打造，支援手機與電腦版面，操作流暢。
* **🧠 智慧結算**：
    * **最佳化方案**：自動抵銷債務，提供最少轉帳次數的建議。
    * **原始帳務**：清楚條列「誰欠誰多少」的詳細清單。
* **☁️ 雲端同步**：整合 Google Firebase，資料即時儲存不遺失。
* **🔒 安全設計**：設定檔分離，確保 API Key 安全。

## 🛠️ 使用技術

* **Frontend**: HTML5, JavaScript (ES6 Modules)
* **Styling**: Tailwind CSS (CDN)
* **Backend / Database**: Google Firebase (Firestore)
* **Hosting**: Firebase Hosting

## 🚀 如何在本地執行 (Getting Started)

如果你想在自己的電腦上運行此專案，請依照以下步驟：

### 1. 下載專案
```bash
git clone [https://github.com/yeega185/Trip-cost-splitting.git](https://github.com/yeega185/Trip-cost-splitting.git)
cd Trip-cost-splitting
```
### 2. 設定 Firebase
本專案依賴 Firebase 運作，你需要建立自己的設定檔：
將 config.example.js 複製一份，並改名為 config.js。
前往 Firebase Console 建立新專案。
啟用 Firestore Database。
取得你的網頁應用程式設定 (SDK Configuration)。
將你的 API Key 等資訊填入 config.js 中：
```bash
// config.js
export const firebaseConfig = {
    apiKey: "你的_API_KEY",
    authDomain: "你的專案ID.firebaseapp.com",
    projectId: "你的專案ID",
    // ... 其他設定
};
```

### 3. 啟動網頁
由於使用了 ES6 Modules (import/export)，直接雙擊 index.html 可能會因為 CORS 政策而無法運作。建議使用以下方式開啟：
使用 VS Code: 安裝 "Live Server" 套件，右鍵點擊 index.html 選擇 "Open with Live Server"。
使用 Firebase Hosting:
```bash
firebase serve
```

Made by Yeega