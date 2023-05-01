# SeLine 

SeLine 是由[Honc](https://blog.honcbb.me/) 安全研究人員個人在閒暇之餘所開發的小工具，並不是由Line 公司或第三方所開發，SeLine 程式是針對Line 通訊軟體的帳戶驗證是否為詐騙，且詐騙Line ID的資料庫是由["政府資料開放平臺"](https://data.gov.tw/dataset/78432) => 內政部警政署165 所提供。

![image](https://i.imgur.com/HKnaPfs.png)

[![Release](https://img.shields.io/badge/%E7%89%88%E6%9C%AC-V1.0-green)](https://github.com/honcbb-secu/SeLine/releases/)

[![Release](https://img.shields.io/badge/%E9%BB%9E%E6%88%91-%E4%B8%8B%E8%BC%89-brightgreen)](https://github.com/honcbb-secu/SeLine/releases/download/V1.0/SeLine.zip)

`SeLine 程式(壓縮檔密碼)：se_line_fkfio3*/45`

## Demo

[![ScreenShot](https://i.imgur.com/GfcJnHw.png)](https://www.youtube.com/watch?v=gM_wgnYeEw4&feature=youtu.be)

## 更新

SeLine 會因程式Bug或者其他原因不定時更新，也在未來**可能**會增加其他功能

## 謹記

SeLine 雖然是一個可查詢Line 帳號是否為詐騙，但這些結果都是取自於["政府資料開放平臺,內政部警政署165"](https://data.gov.tw/dataset/78432) 所通報並公開數據資料所引用，並未有提前預知或者自動判斷是否為詐騙之功能，[SeLine](https://github.com/honcbb-secu/SeLine) 與[趨勢科技防詐達人](https://getdr.com/) 功能有點類似；但後者**趨勢科技防詐達人**支援比較廣泛全面且應用功能較多。

## 支援

Windows系統

## 分析

SeLine 查詢驗證結果則使用[**"政府資料開放平臺,內政部警政署165"**](https://data.gov.tw/dataset/78432) 所公開的**詐騙Line ID**資料來驗證，在傳輸過程當中所有**客戶端**資料都是直接與本地數據資料作比對（**並未將所輸入資訊傳至作者伺服器或者其他第三方伺服器！**) 因此非常安全！

## 安全

作者同樣依照以往慣例，也為了保護軟體安全因而採用**軟體加密保護技術**，所以有些防毒軟體產品會判**SeLine**為是惡意木馬部分，但同樣可保證是**SeLine** 絕沒有植入**病毒木馬**及**竊取用戶電腦資訊** 任何情況，如果還是**無法放心(請勿使用)**

## 如何使用？

把疑似您認為是詐騙的Line 帳戶並知道對方Line ID 情況下，將Line ID 輸入至程式介面的**輸入框** 再點選**檢查** 後等待結果通知即可。

## 常見問題

* 為什麼開啟程式出現**請先確定是否有連線！** ? 

    → 『因為程式加入了相關版本驗證通知必須與伺服器作連線確認，因此前提開啟程式下必須先開啟網路執行才行』
    
* 為什麼開啟程式出現**程式已有更新版本或政府提供數據資料位置已變更！將在確定後自動下載新版本至目前位置，請重新執行。** ? 

    → 『程式已經有新功能或修正其他相關錯誤Bug 或政府提供的數據資料位置有變更而衍生出新版本，此時只需在提示視窗點選"確定"後將自動從伺服器上下載最新SeLine.zip 只需解壓縮重新執行即可。』
    
* 為什麼開啟程式出現**元件'MSInet.ocx'或它的依存檔案並未正確地註冊:某檔案遺漏或不正確** ? 

    → 『這個錯誤是因為SecVir 程式本身引用了網路驗證MSInet.ocx 組件，必須要有這個檔案才能正確與伺服器驗證並且回傳相關通知訊息，電腦處於兩種情況：
    
    一. 電腦路徑C:\Windows\SysWOW64\* 沒有這個MSInet.ocx檔案，所以須至網路尋找並放置正確路徑即可>[可點我下載](https://www.ocxme.com/files/msinet_ocx)
    
    二. 電腦雖有這個檔案，但沒有給它正確註冊，可參考[這篇文章](https://dotblogs.com.tw/usice0314/2010/04/07/14442) 修改一下註冊即可』
  
* 查詢結果是可信的嗎？這些結果都是怎麼樣驗證的？
 
  → 『SeLine 是調用["政府資料開放平臺,內政部警政署165"](https://data.gov.tw/dataset/78432) 公開詐騙LineID數據集資料(結果請以內政部165 政府機關所提供結果為主) 』
  
* 一定要連線才能開啟程式(查詢) 使用? 
 
  → 『是的，因為程式都會至政府資料開放平臺下載最新的數據至本地且程式會驗證是否為新版本，然而必須連網才能。 』
  
* 我很確切某個帳戶是詐騙的，但是為什麼程式顯示"非詐騙"? 
 
  → 『因為內政部165 機關提供的資料都是經由查證或者民眾所通報才會公開，若您確認所輸入Line ID 為詐騙（但程式顯示非詐騙），請至(https://165.npa.gov.tw/#/) （名.內政部警政署165全民防騙網) 循正當管道舉報供政府機關審核。 』
  
* 本程式僅是直接調用.csv 中資料，並將所有資料篩選並統一與用戶輸入作比較而顯示＂驗證結果＂。
  
 
 ## 聯絡

若有任何問題請聯繫我：honcbb@gmail.com
  
  
