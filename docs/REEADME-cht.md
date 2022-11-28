# Stable Diffusion webui for Colab & 匯入外部模組

# [English](../README.md) | 繁體中文

<br>本專案會引導您添加預先訓練模組 (ckpt/vae)

## 前言
automatic1111 讓一般使用者可以利用 Colab 雲端運算來體驗 AI繪圖。<br>
那除了預設的模組外，社群也提供相當多樣的訓練模組。<br>
可是模組很大、而且GDrive不適合放模組... -_-


# 在開始之前
我們都知道，Colab免費版提供GPU與存儲空間供開發人員利用，但沒有資源保底。<br>
基本上，Tesla T4 、 大約 10~12GB 的 RAM 、還有 60~90GB 的硬碟空間。
<br> **請妥善利用空間**
<br>

# 您需要備妥
 * 一個 Google 帳號可以存取 Colab 。
 * 掛載硬碟的權限 (可選)
 * 一個 PixelDrain 帳號  (可選)

# 模型存放位置
筆者將模組檔案上傳 PixelDrain (不是推銷)<br>
該空間會保留檔案 60 天 (如果無人存取、則會刪除)<br>
下載速度約 6~20MB/s by cUrl in colab. (如果我找到更好的免空會改掉)

# 如何匯入模組
```
Model
curl -Lo <name>.ckpt <path/to/PixelDrain/Link>
Vae weight
curl -Lo <name>.vae.pt <path/to/PixelDrain/Link>
```
\<name> 與模組名相同，例如： `stable-diffusion-V1.4-puned.ckpt`. <br>
\<path/to/PixelDrain/Link> is "https://pixeldrain.com/api/file/`your-shared-link`?download"
 <br> 我提供的 webui 筆記本使用的模組是 `Anything-V3.0` 調和 `dbMai` 比例是 65% 
 <br>由我提供 (我推薦該風格！)

 # 功能改進
 我提供的 jupyter 筆記本可以將您的創意產出利用 zip 匯出到您的硬碟 (依照日期產生 yyyy-mm-dd-H-m.zip )

 ## 更多資訊
 模組清單 <br>
https://rentry.org/sdmodels