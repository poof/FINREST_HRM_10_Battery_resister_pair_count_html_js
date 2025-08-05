# FINREST_HRM_10_Battery_resister_pair_count_html_js
上傳HRM-10的CSV檔案HISTORY.CSV(電池量測內阻清單)，或是簡易輸入電池內阻，一行一個，
選擇你要的電池組串並聯組合， 就可以自動產生電池組配對表， 讓每一組電池的內阻相近， 並且可以視覺化呈現電池的內阻、電壓。

"Upload the CSV file HISTORY.CSV (battery internal resistance measurement list) for HRM-10, or simply input the internal resistance values, one per line. Then, select your desired series-parallel combination for the battery pack. The system will automatically generate a battery pack pairing list, ensuring that the internal resistance of each battery group is similar. Additionally, it will provide a visual representation of the batteries' internal resistance and voltage."

[線上Online](https://void.ics.app/cdn/battery_matcher_i18n.html)

# 電池配對工具 - 使用說明

## Battery Cell Matching Tool - User Guide

### 如何使用 (How to Use)

1.  **開啟檔案 (Open the File):**
    *   在您的網頁瀏覽器中開啟 `battery_matcher_i18n.html` 檔案。
    *   **In your web browser, open the `battery_matcher_i18n.html` file.**

2.  **切換語言 (Switch Language):**
    *   點擊頁面右上角的 **中文 / English** 來選擇您偏好的語言。
    *   **Click "中文 / English" in the top-right corner to select your preferred language.**

3.  **載入資料 (Load Data):**
    *   **方式一 (Option 1):** 點擊 **"上傳 CSV 檔案"** 按鈕，選擇您的 `HISTORY.CSV` 資料檔。
    *   **方式二 (Option 2):** 直接複製您 CSV 檔案的全部內容，貼到下方的文字框中。
    *   資料載入後，下方的篩選器會自動填上預設值。
    *   **方式三 (Option 3):** 簡易輸入電池內阻毫歐姆(mΩ)，一行一個。

4.  **設定配對參數 (Configure Parameters):**
    *   在 **"串數 (S)"** 和 **"並數 (P)"** 欄位輸入您想要的電池組規格 (例如 6S3P)。

5.  **(可選) 設定篩選條件 (Optional - Set Filters):**
    *   **群組篩選:** 取消勾選您不想納入計算的電池批次 (Group)。
    *   **狀態篩選:** 勾選 "納入FAIL電池" 來包含不合格的電池。
    *   **範圍篩選:** 勾選啟用電壓或內阻篩選，並修改最小/最大值來縮小電池選擇範圍。

6.  **計算與檢視結果 (Calculate and View Results):**
    *   點擊 **"計算與視覺化"** 按鈕。
    *   下方的 **配對結果** 和 **視覺化圖表** 將會立即產生。
---

### CSV 檔案格式需求 (Required CSV Format)

-   您的 CSV 檔案需要包含 `No.`, `Group`, `Result`, `Voltage`, `Resistor` 這幾個欄位。
-   **Your CSV file must contain the following columns: `No.`, `Group`, `Result`, `Voltage`, `Resistor`.**

**範例 (Example):**
```csv
No.,Group,Result,Voltage,Resistor,Date,Time
1,M3,PASS,4.1906,0.0196,2025/08/06,00:47:09
2,M3,PASS,4.1940,0.0181,2025/08/06,00:47:22
...
```

<img width="410" height="442" alt="image" src="https://github.com/user-attachments/assets/e69ccdba-f06c-4358-a752-177814010005" />
<br>
<img width="419" height="403" alt="image" src="https://github.com/user-attachments/assets/ec6902c3-8106-47fe-8b5f-3dc9b837b88a" />
<br>
<img width="410" height="206" alt="image" src="https://github.com/user-attachments/assets/2ad69c9d-462e-4140-a14d-9acf4330b9b3" />
<br>
<img width="419" height="416" alt="image" src="https://github.com/user-attachments/assets/bcee246f-3eaf-48f3-bf40-6f9e9daf0cbf" />



