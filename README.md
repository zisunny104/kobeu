# KoiLiSu KoBeU - 課表下載器

> 亞洲大學學生課表下載工具

## 介紹

KoiLiSu KoBeU（課表下載器）是專為亞洲大學學生設計的課表下載工具，支援 PDF 和 Excel 兩種格式的批次下載。

## 特色

✅ **雙格式支援**：PDF 和 Excel 課表  
✅ **批次下載**：支援多學號同時處理  
✅ **學年期設定**：靈活設定學年期  
✅ **現代化介面**：基於 Tocas UI 5.0.3  
✅ **深淺色主題**：支援主題切換  
✅ **響應式設計**：適配各種裝置  

## 使用方法

1. 設定學年期（例如：1141）
2. 輸入學號（支援多個，用逗號或空格分隔）
3. 系統自動驗證學號格式（9位數字）
4. 選擇下載格式：
   - PDF 課表：標準格式課表
   - Excel 課表：可編輯的電子表格格式

## 技術說明

### PDF 下載 URL

```
https://cosinfo.asia.edu.tw/cosinfo/system/Print/asycoslessonrpt.asp?smtr={學年期}&deptno=&sel_txt={學號}&rptno=std&cos_year=&cos_class=undefined&building=&ne=&clsnum=undefined&rpt=
```

### Excel 下載 URL

```
https://cosinfo.asia.edu.tw/cosinfo/system/COS/showExcel.aspx?rptname=showword&Tname={學號}&smtr={學年期}&deptno=&sqlstr=exec roomclass_v2_sp '{學年期}','{學號}','std','','',''
```

## 安裝

### 獨立使用

1. Clone repo：
```bash
git clone https://github.com/zisunny104/kobeu.git
cd kobeu
```

2. 配置網頁伺服器

3. 直接訪問 `index.php`

### 與 KoiLiSu 開利手整合

1. 將此 repo 放置在 `koilisu/apps/kobeu/` 目錄
2. 透過 `https://toka.dev/koilisu/kobeu` 造訪

## 版本歷史

### v1.7.1
- 升級至 Tocas UI 5.0.3
- 優化使用者介面
- 改進響應式設計
- 增強主題切換功能

### v1.6.x
- 支援批次下載
- Excel 格式支援
- 現代化介面升級

## 學年期對照

| 學年期代碼 | 對應學期 |
|------------|----------|
| 1131 | 113學年第1學期 |
| 1132 | 113學年第2學期 |
| 1141 | 114學年第1學期 |
| 1142 | 114學年第2學期 |

## 系統需求

- PHP 7.4+
- 現代瀏覽器
- 需要校內網路或 VPN 連線

## 注意事項

⚠️ 此工具僅適用於亞洲大學學生使用  
⚠️ 需要校內網路環境或 VPN 連線  
⚠️ 請遵守學校相關規定使用  
⚠️ 學年期格式：YYYQ（YYY為民國年，Q為學期）  

## 授權

MIT License，詳見 [LICENSE](LICENSE)。

## 作者

Tokas (Xiang-zi Xie)